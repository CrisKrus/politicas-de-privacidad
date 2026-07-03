# Políticas de Privacidad

GitHub Pages público con las políticas de privacidad de las aplicaciones desarrolladas por [CrisKrus](https://github.com/CrisKrus).

## URL pública

La página está disponible en: `https://criskrus.github.io/politicas-de-privacidad/`

## Estructura

```
.
├── index.md              # Página de inicio con la lista de apps
├── template/
│   └── politica-de-privacidad.md   # Plantilla para nuevas apps
└── apps/
    └── <nombre-app>.md  # Política de privacidad de cada app
```

## Cómo añadir la política de privacidad de una nueva app

1. Copia la plantilla en la carpeta `apps/`:
   ```bash
   cp template/politica-de-privacidad.md apps/nombre-app.md
   ```
2. Edita el archivo copiado y remplaza los marcadores:
   - `NOMBRE_APP` → nombre real de la aplicación
   - `DESCRIPCIÓN_BREVE_DE_LA_APP` → descripción de una línea
   - Completa cada sección con los detalles de privacidad de tu app.
3. Añade un enlace en `index.md`:
   ```markdown
   - [Nombre de la App](./apps/nombre-app.md)
   ```
4. Haz commit y push. GitHub Pages publicará los cambios automáticamente.

## Configuración de GitHub Pages

Asegúrate de que GitHub Pages esté habilitado en la configuración del repositorio
(**Settings → Pages**) apuntando a la rama `main` y al directorio raíz `/`.
