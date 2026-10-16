# Tags HTML

<p align="center">
  <img src="assets/img/logo-tags-html.png" alt="Tags HTML" width="420">
</p>

<p align="center">
  <strong>Guía visual de las principales etiquetas de HTML5: qué hace cada una, cómo se escribe y cómo se ve al renderizarse.</strong>
</p>

<p align="center">
  <a href="https://tagshtml.vercel.app"><img src="https://img.shields.io/badge/demo-tagshtml.vercel.app-E0451B?style=flat-square" alt="Demo en Vercel"></a>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/sin%20dependencias-000000?style=flat-square" alt="Sin dependencias">
</p>

Página web estática y educativa que documenta **37 etiquetas de HTML5**. Para cada una muestra su definición, el código que la usa y un ejemplo práctico renderizado en el navegador, siguiendo siempre el mismo patrón de lectura.

> [!TIP]
> ¿Solo quieres verla? Está publicada en **[tagshtml.vercel.app](https://tagshtml.vercel.app)**.

## Características

- **37 etiquetas documentadas**, agrupadas por tipo, con definición, bloque de código y resultado visible.
- **Índice fijo** con resaltado automático de la entrada activa mediante `IntersectionObserver`.
- **Diseño adaptable**: retícula de dos columnas en escritorio y una sola columna con índice plegable en móvil.
- **Accesibilidad**: enlace para saltar al contenido, foco visible, `aria-label` en la navegación y respeto por `prefers-reduced-motion`.
- **Sin dependencias**: solo HTML y CSS, sin build ni instalación. Las tipografías se cargan desde Google Fonts y caen a las fuentes del sistema si no hay conexión.

## Contenido

El documento recorre las etiquetas en cuatro secciones:

- **Texto y encabezados:** `h1`–`h6`, `p`, `br`, `wbr`, `pre`, `blockquote`, `small`, `u`, `mark`, `ins`, `del`, `sub`, `sup`, `time`, `data`, `dfn`, `code`, `samp`, `kbd`
- **Estructura semántica:** `main`, `section`, `article`, `header`, `footer`, `aside`, `nav`, `figure`, `figcaption`, `div`
- **Multimedia y gráficos:** `img`, `svg`
- **Tablas:** `caption`, `colgroup`, `col`, `thead`, `tbody`, `tfoot`

## Estructura del proyecto

```
tags_html/
├── index.html                     # Documento principal con las 37 entradas
├── README.md
├── .gitignore
└── assets/
    ├── css/
    │   └── tags-html.css          # Tokens, retícula y componentes
    └── img/
        ├── logo-tags-html.png     # Logotipo de la cabecera
        ├── favicon.png            # Icono y ejemplo de figcaption
        ├── estructura-pagina.jpg  # Diagrama de estructura (entrada section)
        ├── diseno-con-div.png     # Ejemplo de diseño con div
        ├── ejemplo-kbd.jpg        # Ejemplo de kbd
        ├── anatomia-img.webp      # Esquema de la etiqueta img
        └── paisaje.jpg            # Imagen de ejemplo de figure
```

## Uso

No requiere instalación ni servidor. Abre el archivo `index.html` directamente en cualquier navegador:

```powershell
Start-Process "index.html"
```

Si prefieres servirlo en local:

```powershell
python -m http.server 8000
```

## Estilos

Los estilos se definen en `assets/css/tags-html.css`:

- Paleta de tokens en `:root`: papel `#ECEEE8`, papel de ejemplo `#E1E4DC`, tinta `#1A1A1A`, grafito `#5D6360`, señal `#E0451B` y filete `#C7CBC2`.
- Tipografía Archivo (con eje de ancho variable para el titular) e IBM Plex Mono para etiquetas y código.
- Retícula de dos columnas: índice fijo a la izquierda y columna de contenido de medida 70ch; a partir de 900px pasa a una sola columna con el índice plegable.

## Demo

El sitio está desplegado en Vercel: **https://tagshtml.vercel.app**

## Autor

Jhoam Sebastian Muñoz B y Cristian Camilo Muñoz B. Todos los derechos reservados.
