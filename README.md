# Café Esquina
Landing de práctica para una cafetería ficticia, creada con React + Vite. Sin dominio propio, base de datos ni backend real.

## Arrancar
Requiere Node.js 22 o superior.
```bash
npm install
npm run dev
```
Abrir la dirección que muestra Vite (normalmente http://localhost:5173).
```bash
npm run build
npm run preview
```
La compilación genera dist/.

## Qué está simulado
- Cafetería, dirección, horarios, carta y precios: ficticios.
- El formulario valida nombre, email y mensaje mediante validación HTML nativa. Simula una espera de 750 ms y muestra confirmación. NO envía correos, NO hace peticiones a un servidor y NO guarda datos.
- No hay reservas, pagos ni tratamiento real de mensajes. Utilizar datos ficticios.
- El requisito «el formulario envía» solo se cumple como simulación; si la revisión exige recepción real, será necesario acordar un servicio de formularios adicional.
- Ilustración SVG propia; fuentes de Google Fonts con alternativas locales.

## Reiniciar datos de ejemplo
Los datos de la carta están en src/main.jsx. No hay almacenamiento persistente: recargar la página reinicia el estado de confirmación. Un envío de prueba correcto vacía el formulario.

## Previsualización Vercel
Importar este repositorio, seleccionar Vite y usar npm run build con salida dist. No requiere variables de entorno. Para revisión pública, comprobar que la URL se abre sin iniciar sesión; las previews pueden tener protección activada.
URL: pendiente de despliegue.

## Revisión manual
- Probar a 375 px y en escritorio: no debe haber desplazamiento horizontal.
- Abrir/cerrar menú móvil y probar los enlaces internos.
- Campos vacíos/email incorrecto deben bloquear el envío.
- Envío válido: estado de espera, botón deshabilitado, confirmación accesible y campos vacíos.
- Recargar: la confirmación desaparece.
- Navegar con teclado.
- Invitar a @kodarvia como colaborador antes de enviar el encargo a revisión.
