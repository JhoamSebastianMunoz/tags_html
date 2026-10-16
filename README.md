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
├── index.html                       # Documento principal con las 37 entradas
├── tags_html.css                    # Hoja de estilos (tokens, retícula, componentes)
├── html-5.png                       # Favicon y ejemplo de figcaption
├── tag_html.png                     # Logotipo de la cabecera
├── Etiquetas HTML5.JPG              # Diagrama de estructura (entrada section)
├── html5_11.png                     # Ejemplo de diseño con div
├── maxresdefault.jpg                # Ejemplo de kbd
├── etiquetas-y-atributos-hmtl-3.webp # Esquema de la etiqueta img
├── seebensee-2384369.jpg            # Imagen de ejemplo de figure
├── html-dfn.png                     # Recurso sin usar
└── htmlsamptag.png                  # Recurso sin usar
```

## Uso

No requiere instalación ni servidor. Abre el archivo `index.html` directamente en cualquier navegador web:

```powershell
Start-Process "index.html"
```

Las tipografías se cargan desde Google Fonts (Archivo e IBM Plex Mono) y caen a las fuentes del sistema si no hay conexión.

## Estilos

Los estilos se definen en `tags_html.css`:

- Paleta de tokens en `:root`: papel `#ECEEE8`, papel de ejemplo `#E1E4DC`, tinta `#1A1A1A`, grafito `#5D6360`, señal `#E0451B` y filete `#C7CBC2`.
- Tipografía Archivo (con eje de ancho variable para el titular) e IBM Plex Mono para etiquetas y código.
- Retícula de dos columnas: índice fijo a la izquierda y columna de contenido de medida 70ch; a partir de 900px se pasa a una sola columna con el índice plegable.
- Ejemplos con código y resultado en el mismo bloque, foco visible, `prefers-reduced-motion` respetado y resaltado de la entrada activa con `IntersectionObserver`.

## Autor

Jhoam Sebastian Muñoz B y Cristian Camilo Muñoz B. Todos los derechos reservados.
