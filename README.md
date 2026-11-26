# PASSHOUSE — Landing pages A/B con formulario de captación visible

## Archivos
- `index.html`: versión A — historial técnico
- `version-b/index.html`: versión B — prevención, diseño oscuro con acentos ámbar, franja ANTES/DURANTE/DESPUÉS y formulario color crema (diseño diferente a A)
- `assets/styles.css`: estilos compartidos
- `assets/app.js`: lógica de formulario compartida
- `assets/logo-passhouse.png`: recorte del logotipo visible en la captura de Google Sites. REEMPLAZAR por el logo original en buena calidad si está disponible.
- `checklist-passhouse.html`: recurso gratuito

## Captación real (obligatorio antes de usar con usuarios reales)
1. Configurar el receptor de formularios compatible con POST JSON y CORS. El ejemplo de AmigoSeguro menciona Formspree.
2. En `assets/app.js` completar `const FORM_ENDPOINT = "https://formspree.io/f/ID_REAL";` con el endpoint público real (no un enlace a la cuenta, ni un secret).
3. En `assets/app.js` completar `const CONTACT_EMAIL = "correo-de-contacto-real";`.
4. Revisar el aviso de privacidad: responsable, contacto, finalidad, servicio receptor y conservación de datos. No publicar una versión inexacta.
5. Probar con datos de prueba desde A y B y verificar recepción (incluido campo `pagina` A/B).
6. Si endpoint o email quedan vacíos, el formulario avisa claramente que NO guarda ni envía datos (modo demostración).

## Publicar sobre el repo existente
1. Ir a github.com/jhonbejarhuamanttupa/passhouse-landing.
2. Mantener el repositorio y usar `Add file > Upload files` (o clonar localmente) para actualizar la raíz con estos archivos y subcarpetas.
3. Comprobar que index.html y version-b/index.html quedaron en las rutas correctas. Cargar también la carpeta assets y checklist-passhouse.html.
4. Confirmar cambios (commit); Pages usará el contenido de la rama main / root configurada.
5. Abrir ambas URL publicadas y comprobar la visibilidad del formulario en móvil y computadora.

## Enlaces esperados
A: https://jhonbejarhuamanttupa.github.io/passhouse-landing/
B: https://jhonbejarhuamanttupa.github.io/passhouse-landing/version-b/

## Evidencia de clase
- Capturas mostrando formulario junto al hero de A y B.
- Prueba de entrada recibida en el servicio de formularios, sin mostrar datos personales reales.
- Dejar explícito que el checklist se abre en el sitio; no se envía por correo automáticamente.

## DIFERENCIAS VISUALES
- A: fondo celeste, cabecera azul, mensaje de orden del historial, formulario blanco, tarjetas informativas.
- B: fondo azul marino oscuro, detalles naranja/ámbar, historia de reparación preventiva, franja ANTES/DURANTE/DESPUÉS, formulario crema de alto contraste y secciones propias.
- Ambos comparten la marca, logo y checklist, pero sus diseños son distintos.

## Google Sites
Crea una sección de Landing Page A y otra de Landing Page B, cada una con un botón hacia las URL públicas de GitHub Pages. En Google Sites > Insertar > Insertar/Embeber > URL puedes probar a incrustar ambas, pero si no se muestra el formulario o se bloquea el marco usa botón que abra la página original. Publica los cambios.
