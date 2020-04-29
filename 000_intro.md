# Introducción VIM

## Configuraciones

**crear un archivo o acceso**
`vim +[número_linea] archivo.txt`

- **Permite descargar el diccionario en español** `set spelllang=es`
- **habilita el corrector ortografico** `set spell`
- **deshabilita el corrector ortografico** `nospell`
- **mostrar los números de linea** `set number`
- **no muestra los números de las lineas** `set nonumber`
- **habilita y deshabilita los números de la lineas** `set number!`
- **permite selecionar un esquema de colores** `colorscheme esquema`
- **Permite visualizar la linea del cursor** `set cursorline`
- **Cambiar el color de linea del cursor** `highlight CursorLine guidb=lightblue ctermbg=blue`
- **Crea un linea del curso en la columna** `set cursorcolumn`
- **Permite deshabilitar vi para reemplazar con las opciones de vim** `set nocompatible`
- **Permite el retroceso, la sangria y el inicio de inserción** `set backspace= indent, eol, start`
- **Establece un numero mayor de comando ejecutados es el historial** `set history=1000`
- **Muestra los comandos en parte inferior escrito en teclado** `set showcmd`
- **Muestra el modo actual en la parte inferior** `set showmode`
- **Vuelve a leer automáticamente los archivos** `set autoread`
- **Ocultas los buffers sin que se escriban en el disco duro, solo se recuerdan y se ven en el historial** `set hidden`
- **Habilita el número de líneas** `set nu`
- `jumps | :ju`


## Abrir, modificar Archivos

- **Permite abrir muchos archivos pero se debe utilizar buffers** `vim [archivo 1] [archivo n]`
- **Permite abrir muchos archivos en ventanas verticales** `vim -o [archivo 1] [archivo n]`
- **Permite abrir muchos archivos en ventanas horizontales** `vim -O  [archivo 1] [archivo n]`
- **Abrir el último documento editado** `Ctrl + o + o`
- **Apretando escape entra modo comando** `Esc`
- **Deshacer cambio** `u`
- **Rehacer cambios** `Ctrl + r`
- **copiar contenido** `y`
- **pegar contenido** `p`
- **cortar contenido** `c`
- **el primero guarda, guarda y termina y el ultimo realizar termino con fuerza** `:w, :wq, :q!`
- **Permite eliminar los espacio o tabulaciones de la sangria en todo el bloque o documento hacia la izquierda del cursor** `=G`

## Abrir multiples archivos

- `vim [archivo 1] [archivo n]`  **Permite abrir muchos archivos pero se debe utilizar buffers**
- `vim -o [archivo 1] [archivo n]`  **Permite abrir muchos archivos en ventanas verticales**
- `vim -O  [archivo 1] [archivo n]`  **Permite abrir muchos archivos en ventanas horizontales**
- **Permite ir saltando en pestañas** `CTRL-w w`
- **Permite ir hacia arriba en las pestañas** `CTRL-w k`
- **Permite ir hacia abajo en las pestañas** `CTRL-w j`
- **Permite ir hacia izquierda en las pestañas** `CTRL-w h`
- **Permite ir hacia derecha en las pestañas** `CTRL-w l`

## Read

- **Inserta el texto el archivo seleccionado** `:r [nombre archivo]`
- **Inserta en el archivo la primera línea del archivo seleccionado.** `:0r [nombre archivo]`
- **Inserta las líneas 2 y 8 del archivo seleccionado en el documento actual.** `:r !sed -n 2,8p [nombre archivo]`
- **Insertar el resultado de comandos, por ejemplo** `:r ![comando]`

### Ejemplos

- `:r !ls` **inserta en el documento el resultado y mostrara el resultado del directorio.**

## Guardar

- **Guardar como** `:sav [nuevo archivo]`
- **Sobreescribir un archivo** `:w! [nombre archivo]`
- **guarda un archivo el buffer o el documento ha sido modificado** `:up[date] [nombre archivo]`
