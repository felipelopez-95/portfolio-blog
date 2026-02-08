# Portafolio personal

Sitio web personal desarrollado con [Astro](https://astro.build) que presenta experiencia laboral, proyectos y una sección sobre mí. El diseño es minimalista, responsive y soporta tema claro y oscuro.

## Características del proyecto

El proyecto se ha construido siguiendo buenas prácticas de desarrollo web. Se ha utilizado asistencia de IA para profundizar en convenciones y patrones recomendados. La estructura se basa en **HTML semántico** (etiquetas como `section`, `article`, `header`, `footer`, `nav`, listas y `figure`) y **CSS** con enfoque **mobile-first** y metodología **BEM** para los nombres de clases. Se han aplicado las recomendaciones de Astro para optimización y mejores prácticas en el uso de componentes y etiquetas.

La interfaz incluye **tema claro y oscuro** controlado desde el header, manejando el DOM para alternar clases y variables CSS. El sitio utiliza transiciones suaves y un diseño responsive que se adapta a distintos tamaños de pantalla.

El código está organizado en **componentes reutilizables** (por ejemplo `SectionTitle`, `Tags`, `ExperienceItem`, `ProjectItem`) con paso de **props** y **renderizado condicional** donde aplica, manteniendo la lógica clara y fácil de mantener.

## Tecnologías

- **Astro** — Framework estático
- **HTML** y **CSS** (variables CSS, flexbox, grid)
- **npm** — Gestión de dependencias y scripts

## Requisitos previos

- [Node.js](https://nodejs.org/) (recomendado v18 o superior)
- npm (incluido con Node.js)

## Clonar y ejecutar en local

1. **Clonar el repositorio**

   ```bash
   git clone https://github.com/felipelopez-95/portfolio-blog.git
   cd portfolio-blog
   ```

2. **Instalar dependencias**

   ```bash
   npm install
   ```

3. **Iniciar el servidor de desarrollo**

   ```bash
   npm run dev
   ```

   La aplicación estará disponible en `http://localhost:4321` (o el puerto que indique la terminal).

4. **Vista previa de la build de producción** (opcional)

   ```bash
   npm run build
   npm run preview
   ```

## Desplegar

El proyecto genera sitio estático. Puedes desplegarlo en cualquier plataforma que sirva archivos estáticos.

### Opción 1: Vercel

1. Conecta tu repositorio de GitHub con [Vercel](https://vercel.com).
2. Vercel detectará Astro. Si no, configura el **Framework Preset** como Astro.
3. Comando de build: `npm run build`.
4. Directorio de salida: `dist`.
5. Despliega. Los siguientes pushes a la rama principal se desplegarán automáticamente.

### Opción 2: Netlify

1. Conecta el repositorio en [Netlify](https://www.netlify.com).
2. Build command: `npm run build`.
3. Publish directory: `dist`.
4. Despliega. Puedes activar deploys automáticos desde tu rama principal.

### Opción 3: Build manual y subida

1. Genera la build en tu máquina:

   ```bash
   npm run build
   ```

2. La carpeta `dist` contendrá los archivos estáticos. Súbelos a tu hosting (FTP, S3, GitHub Pages, etc.) según las instrucciones del proveedor.

## Scripts disponibles

| Comando           | Descripción                    |
| ----------------- | ------------------------------ |
| `npm run dev`     | Servidor de desarrollo         |
| `npm run build`   | Genera el sitio en `dist`      |
| `npm run preview` | Sirve la carpeta `dist` en local |

## Licencia

Proyecto de uso personal. Si reutilizas ideas o código, se agradece mención al autor.
