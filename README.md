# eriktory.com

Sitio web personal de Erik Tory, consultor estratégico. Presenta servicios de estrategia, tecnología e IA y la propuesta de ecosistemas digitales.

## Stack

- [Astro](https://astro.build/) (salida estática)
- [Tailwind CSS](https://tailwindcss.com/) vía `@tailwindcss/vite`
- TypeScript
- Despliegue automático en GitHub Pages

## Requisitos

- Node.js >= 22
- npm

## Comandos

| Comando                | Descripción                                 |
| ---------------------- | ------------------------------------------- |
| `npm install`          | Instala dependencias                        |
| `npm run dev`          | Servidor de desarrollo en `localhost:4321`  |
| `npm run build`        | Genera el sitio estático en `dist/`         |
| `npm run preview`      | Vista previa del build                      |
| `npm run check`        | Comprueba tipos y errores con `astro check` |
| `npm run lint`         | Ejecuta ESLint                              |
| `npm run format`       | Formatea con Prettier                       |
| `npm run format:check` | Verifica el formato sin modificar archivos  |

## Estructura

```text
src/
├── assets/        Imágenes procesadas por Astro
├── components/    Componentes de Header, Footer y Main
├── layouts/       Layout base
├── pages/         Rutas (index, 404)
└── styles/        Estilos globales y tema de Tailwind
```

## Despliegue

Cada push a `main` ejecuta el workflow de CI (lint, check y build) y el de despliegue a GitHub Pages (`.github/workflows/deploy.yml`).
