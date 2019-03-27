# Mol Grid
Administra los tamaños de los contenedores, tamaño de las celdas, su alineación, el espacio entre las ellas y la cantidad de celdas por fila o columna utilizando las propiedades de Flexbox.
__
*Este proyecto utiliza [mol.normalize](https://github.com/mol-project/mol.normalize)*


## Uso e instalación
Para utilizar el grid en tu proyecto, puedes installarlo con [npm](https://www.npmjs.com/)
```sh
npm install https://github.com/mol-project/mol.grid.git
```
importa el archivo principal
```sh
@import '~mol.grid/scss/grid.scss';
```
y crea un archivo que contenga las mismas variables que las que se encuentran en
el archivo de `~mol.grid/scss/_vars.scss`

ó si no tienes tiempo, importa el archivo minificado en tu hoja de estilos principal
```sh
@import '~mol.grid/dist/grid.min.css';
```


## Dev
Clona el repositorio
```sh
git clone https://github.com/mol-project/mol.grid.git
cd mol.grid/
npm install
```
Edita los archivos dentro de la carpeta de **scss**

#### Scripts
- `npm run dist` Actualiza los archivos minificados de la carpeta de distribución **dist**
- `npm run docs` Levanta un servidor local que se autorefresca con los cambios que se ejecuten en los archivos **scss** y actualiza los archivos de **docs**

#### Archivos
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

#### Variables
```text
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans|Open+Sans|PT+Serif');

$m-background:      #fff;
$m-color:           #222029;
$m-primary:         #32bdc6;

$m-font-serif:      'PT Serif', serif;
$m-font-family:     'Open Sans', sans-serif;
$m-font-size:       16px;
$m-font-weight:     400;
$m-letter-spacing:  normal;
$m-line-height:     1.5em;

$m-code-family:     monospace;

$m-h-family:        'Josefin Sans', sans-serif;
$m-h-size:          23px;
$m-h-height:        1em;
$m-h-spacing:       normal;
$m-h-weight:        600;
$m-h-style:         normal;
$m-h-transform:     normal;

$m-spacelement:     20px;

$m-spacebase:       40px;
$m-spacevariations: 10;
$m-grid:            10;

$m-queries:
  (xxs, 1rem,   29.999rem,  80%, inherit, inherit),
  (xs,  30rem,  47.999rem,  80%, inherit, inherit),
  (sm,  48rem,  63.999rem,  80%, inherit, inherit),
  (md,  64rem,  74.999rem,  70%, inherit, inherit),
  (lg,  75rem,  89.999rem,  70%, inherit, inherit),
  (xl,  90rem,  119.999rem, 60%, inherit, inherit),
  (xxl, 120rem, 9999rem,    60%, inherit, inherit);

```
