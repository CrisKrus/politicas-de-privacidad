# Políticas de Privacidad

GitHub Pages público con las políticas de privacidad de las aplicaciones desarrolladas por [CrisKrus](https://github.com/CrisKrus).

## URL pública

La página está disponible en: `https://criskrus.github.io/politicas-de-privacidad/`

## Estructura

```
.
├── index.html                          # Página de inicio con la lista de apps
├── template/
│   └── politica-de-privacidad.html    # Plantilla para nuevas apps
└── <nombre-app>/
    └── politica-de-privacidad.html    # Política de privacidad de cada app
```

## Cómo añadir la política de privacidad de una nueva app

1. Crea una carpeta con el nombre de la app (en minúsculas y sin espacios), por ejemplo `mi-app`.
2. Copia la plantilla dentro de esa carpeta:
   ```bash
   cp template/politica-de-privacidad.html mi-app/politica-de-privacidad.html
   ```
3. Edita el archivo copiado y remplaza los marcadores:
   - `NOMBRE_APP` → nombre real de la aplicación
   - `FECHA` → fecha de última actualización (por ejemplo `3 de julio de 2026`)
   - `CORREO_CONTACTO` → dirección de correo de contacto
   - Ajusta las secciones con los detalles de privacidad de tu app.
4. Añade un enlace a la nueva política en `index.html`, dentro de la lista `<ul>`:
   ```html
   <li><a href="./mi-app/politica-de-privacidad.html">Mi App</a></li>
   ```
5. Haz commit y push. GitHub Pages publicará los cambios automáticamente.

## Configuración de GitHub Pages

Asegúrate de que GitHub Pages esté habilitado en la configuración del repositorio
(**Settings → Pages**) apuntando a la rama `main` y al directorio raíz `/`.
