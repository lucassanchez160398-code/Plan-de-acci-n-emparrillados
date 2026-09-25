# Emparillados · Plan de arranque

Página de seguimiento del plan de 5 semanas, editable entre todos los socios.

- `index.html` — la página.
- `api/state.js` — guarda y lee los cambios en la base de datos (Upstash Redis, conectada desde Vercel).

## Puesta en marcha (una sola vez)

1. **Subir a GitHub:** en el repositorio, *Add file → Upload files*, arrastrar `index.html`, `README.md` y la carpeta `api`, y tocar *Commit changes*. Tienen que quedar en la raíz del repositorio (no dentro de otra carpeta).
2. **Base de datos:** en Vercel, proyecto → *Storage* → *Create Database* → Upstash (Redis), plan gratuito → conectarla al proyecto.
3. **Clave del equipo (opcional):** *Settings → Environment Variables* → `EDIT_PIN` con la clave que quieran. Sin clave, cualquiera con el link puede editar.
4. **Redeploy:** *Deployments* → último deploy → *Redeploy*, para que tome la base y la clave.
5. **Probar:** cambiar el estado de una tarea, esperar "Guardado ✓" y recargar.

Si arriba aparece "Falta conectar la base de datos en Vercel", falta el paso 2 o el redeploy.
