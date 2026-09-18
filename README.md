# Origen — Astro

Migración inicial del sitio HTML/CSS/JS de Origen a Astro.

## Requisitos

- Node.js 18.17 o superior
- npm

## Ejecutar en local

```bash
npm install
npm run dev
```

Luego abre la URL que muestre Astro, normalmente `http://localhost:4321`.

## Estructura

- `src/pages/` — páginas y rutas.
- `src/layouts/` — layouts compartidos.
- `src/components/` — componentes reutilizables.
- `public/` — imágenes, fuentes, CSS y JS heredados del proyecto original.

## Rutas iniciales

- `/`
- `/servicios`
- `/proyectos`
- `/nosotros`
- `/contacto`

## Build de producción

```bash
npm run build
npm run preview
```

La carpeta generada es `dist/`.

## Nota sobre el CSS y JS

La migración conserva inicialmente los archivos originales `css/*.min.css` y `js/*.min.js` en `public/` para minimizar cambios visuales y de comportamiento. Una vez comprobado que todo funciona, pueden ir migrándose a componentes y módulos de Astro de forma gradual.

## Importante sobre videos

El HTML original contiene referencias a archivos dentro de `video/`, pero esa carpeta no estaba incluida en el ZIP recibido. La estructura de Astro queda lista para servirlos: si tienes esos archivos, crea `public/video/` y copia allí los videos correspondientes.
