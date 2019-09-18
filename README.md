# Mol Grid
Administra los tamaños de los contenedores, tamaño de las celdas, su alineación, el espacio entre las ellas y la cantidad de celdas por fila o columna utilizando las propiedades de Flexbox.

*This project is for management of everything you need from a grid. Is Flexbox based. You can edit all about your grid via variables*

## Para usar la librería *How to use* ##
Instala la librería *Install the library*

```sh
npm install https://github.com/mol-project/mol.grid.git
```
Crea o copia el archivo de [variables](https://github.com/mol-project/mol.grid/blob/master/scss/_vars.scss) para editar los media queries, el espaciado y la cantidad de filas que requieres
*Create a var file like [this file](https://github.com/mol-project/mol.grid/blob/master/scss/_vars.scss) where you can edit general style aspects*

En el archivo general de SCSS de tu proyecto, importa el archivo de variables y el archivo principal de la librería *Import the vars and main files in to your project scss file*
```sh
@import '_vars.scss';
@import '~mol.grid/scss/_grid.scss';
```

Y compilalo con el resto de tu código, para evitar cargar tantos archivos. *Compile this with your code and avoid to load a lot of files*

## Archivo de distribución *Distribution File* ##
Descarga el archivo de distrubución y usalo en el head de tu proyecto. *Download the distribution file and added into your head project*
[mol.grid](https://raw.githubusercontent.com/mol-project/mol.grid/master/dist/grid.min.css)
```sh
<link rel="stylesheet" href="mol.grid.css">
```

---

### Archivos ###
```text
mol.grid/
├── dist/
│   ├── grid.min.css
│   └── grid.min.css.map
├── docs/
│   ├── grid.css
│   ├── grid.css.map
│   └── index.html
└── scss/
    ├── _cols.scss
    ├── _containers.scss
    ├── _display.scss
    ├── _flex.scss
    ├── _grid.scss
    ├── _margins.scss
    ├── _paddings.scss
    ├── _rows.scss
    ├── _spacing.scss
    ├── _vars.scss
    └── grid.scss
```

### Variables ###
```text
// mol.normalize // mol.grid
$m-queries: (
  "phone": (
    "since": 320px,
    "until": 767px,
    "width": 90%,
    "minwidth": inherit,
    "maxwidth": inherit,
    "height": auto,
    "minheight": 100vh,
    "maxheight": auto
  ),
  "tablet": (
    "since": 768px,
    "until": 1024px,
    "width": 90%,
    "minwidth": inherit,
    "maxwidth": inherit,
    "height": auto,
    "minheight": 100vh,
    "maxheight": auto
  ),
  "laptop": (
    "since": 1025px,
    "until": 1599.99px,
    "width": 90%,
    "minwidth": inherit,
    "maxwidth": inherit,
    "height": auto,
    "minheight": 100vh,
    "maxheight": auto
  ),
  "desktop": (
    "since": 1600px,
    "until": 99999px,
    "width": 90%,
    "minwidth": inherit,
    "maxwidth": inherit,
    "height": auto,
    "minheight": 100vh,
    "maxheight": auto
  )
);

// mol.core // mol.grid
$m-spacelement: 20px;

// mol.grid
$m-spacebase: 40px;
$m-spacevariations: 10;
$m-grid: 10;
```
