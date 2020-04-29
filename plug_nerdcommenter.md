# NerdCommenter

 Es un plugin para realizar comentarios en vim, se debe realizar la siguiente configuración.
```js
 let mapleader ","
 set timeout timeoutlen = 1500
```
* **,cc** : Para activar el comentario se debe teclear
* **,ci** : descomentar la línea
* **,c+<tecla_espaciadora>** : permite alternar los sacar o colocar comentario
* **,cu** sirve igual para descomentar lineas

la Configuracion es la siguiente:
```zsh
 zsh
" Add spaces after comment delimiters by default

let g:NERDSpaceDelims = 1

"
Use compact syntax for prettified multi-line comments
let g:NERDCompactSexyComs = 1

" Align line-wise comment delimiters flush left instead of following code indentation
let g:NERDDefaultAlign = 'left'
```
