# Shield & Attack 2026

Sitio estático de un solo archivo (`index.html`), sin compilación. Datos en Supabase (`htdelrjulawkqkfayybs`).

## Archivos
- `index.html`: la app completa (datos, lógica y estilos)
- `vercel.json`: sin build + cabeceras de seguridad (CSP, HSTS, no indexar)
- `.gitignore`

## Publicar
Repo **privado** en GitHub → Vercel importa el repo (Framework: Other) → Deploy.
Después cambia `https://REEMPLAZA-CON-TU-DOMINIO.vercel.app` en `vercel.json` por tu dominio real.

## Actualizar
Reemplaza `index.html` en el repo y haz commit; Vercel redespliega solo.

## Pendientes
- Rotar la contraseña del rol `shield_reader`
- Borrar la función vieja `sa-sync-valvoline` y el cliente de prueba "pepe"
- Escapar el HTML de los nombres de clientes antes de pintarlos (hoy no se escapa)

## Seguridad
El visor es abierto: quien tenga la URL ve los datos (incluye los 48 clientes del Excel). Usa repo privado.
