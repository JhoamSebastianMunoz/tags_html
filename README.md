# Tags HTML

Página web estática educativa que documenta y ejemplifica las principales etiquetas de **HTML5**, mostrando para cada una su uso, características, el código que la usa y un ejemplo práctico renderizado en el navegador.

## Contenido

El documento recorre 37 etiquetas agrupadas en cuatro secciones:

- **Texto y encabezados:** `h1`–`h6`, `p`, `br`, `wbr`, `pre`, `blockquote`, `small`, `u`, `mark`, `ins`, `del`, `sub`, `sup`, `time`, `data`, `dfn`, `code`, `samp`, `kbd`
- **Estructura semántica:** `main`, `section`, `article`, `header`, `footer`, `aside`, `nav`, `figure`, `figcaption`, `div`
- **Multimedia y gráficos:** `img`, `svg`
- **Tablas:** `caption`, `colgroup`, `col`, `thead`, `tbody`, `tfoot`

Cada entrada sigue el mismo patrón: definición, bloque de código y resultado visible.

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

No requiere instalación ni servidor. Abre el archivo `index.html` directamente en cualquier navegador web:

```powershell
Start-Process "index.html"
```

Las tipografías se cargan desde Google Fonts (Archivo e IBM Plex Mono) y caen a las fuentes del sistema si no hay conexión.

## Estilos

Los estilos se definen en `assets/css/tags-html.css`:

- Paleta de tokens en `:root`: papel `#ECEEE8`, papel de ejemplo `#E1E4DC`, tinta `#1A1A1A`, grafito `#5D6360`, señal `#E0451B` y filete `#C7CBC2`.
- Tipografía Archivo (con eje de ancho variable para el titular) e IBM Plex Mono para etiquetas y código.
- Retícula de dos columnas: índice fijo a la izquierda y columna de contenido de medida 70ch; a partir de 900px se pasa a una sola columna con el índice plegable.
- Ejemplos con código y resultado en el mismo bloque, foco visible, `prefers-reduced-motion` respetado y resaltado de la entrada activa con `IntersectionObserver`.

## Autor

Jhoam Sebastian Muñoz B y Cristian Camilo Muñoz B. Todos los derechos reservados.
