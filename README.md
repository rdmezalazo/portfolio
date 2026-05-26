# Portafolio Profesional — Ronald Meza Lazo

Portafolio web profesional que muestra los proyectos públicos de GitHub de forma dinámica.

## Características

- **Actualización automática**: Los repositorios se cargan dinámicamente desde la API de GitHub cada vez que se visita el sitio
- **Diseño moderno**: UI dark theme con animaciones suaves, responsive y accesible
- **Sin dependencias de build**: HTML/CSS/JS puro, listo para GitHub Pages
- **Filtrado automático**: Excluye repos específicos (infosolutions, rdmezalazo, cv-ronaldmeza)
- **Descripciones enriquecidas**: Descripciones personalizadas para proyectos conocidos

## Despliegue

Este sitio está diseñado para funcionar con [GitHub Pages](https://pages.github.com/):

1. Ve a **Settings → Pages** en el repositorio
2. En **Source** selecciona `Deploy from a branch`
3. Selecciona la rama `main` y la carpeta `/ (root)`
4. Guarda y espera a que se despliegue

## Personalización

Para modificar los repos excluidos o agregar descripciones personalizadas, edita las constantes al inicio del `<script>` en `index.html`:

```js
const EXCLUDED_REPOS = ['infosolutions', 'rdmezalazo', 'cv-ronaldmeza'];

const REPO_DESCRIPTIONS = {
    'nombre-repo': 'Descripción personalizada',
};
```

## Tecnologías

- HTML5 semántico
- Tailwind CSS (CDN)
- Font Awesome 6 (CDN)
- GitHub REST API v3
- JavaScript vanilla (ES6+)
