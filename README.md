# Mol Grid
Administra los tamaños de los contenedores, tamaño de las celdas, su alineación, el espacio entre las ellas y la cantidad de celdas por fila o columna utilizando las propiedades de Flexbox.

( ﾟ▽ﾟ)/ Hi! [@MolFramework](https://twitter.com/MolFramework)


## Uso e instalación
Para utilizar el grid en tu proyecto, puedes installarlo con [npm](https://www.npmjs.com/)
```sh
npm install --save https://github.com/MolFramework/mol.grid.git
```
e importarlo en tu hoja de estilos principal, éste archivo contiene el archivo del normalize incrustado en el archivo de distribución del módulo grid
```sh
@import '~mol.grid/dist/grid.min.css';
```
o si prefieres utilizar tu propio archivo de variables, importa
```sh
@import '~mol.grid/scss/_grid.scss';
```
y crea un archivo que contenga las mismas variables que las que se encuentran en
el archivo de `~mol.grid/scss/_vars.scss`


## Dev
Clona el repositorio
```sh
git clone https://github.com/MolFramework/mol.grid.git
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

#### Variables específicas del grid
```text
$m-queries:
    (xxs, 1rem, 29.999rem, 80%, inherit, inherit),
    (xs, 30rem, 47.999rem, 90%, inherit, inherit),
    (sm, 48rem, 63.999rem, 90%, inherit, inherit),
    (md, 64rem, 74.999rem, 90%, inherit, inherit),
    (lg, 75rem, 89.999rem, 80%, inherit, inherit),
    (xl, 90rem, 119.999rem, 75%, inherit, inherit),
    (xxl, 120rem, 9999rem, 70%, inherit, inherit);

$m-spacebase: 40px;
$m-spacevariations: 10;
$m-grid: 10;
```
