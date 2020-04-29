# Tips con VIM

- `/v/`*expresion_regular*`/d`  **Borrar rangos con regex**
- `vap`  **podra seleccionar un parrafo**
- `Ctrl + o + o`  **abre el último documento editado**
- `J`  **Permite unir una selección de frase o palabras de diferentes líneas de una sola**
- `Shift + 5`  **Pemite saltar de un simbolo de apertura hacia el simbolo de cierre y viceversa**
- **Listar 1000 número de lineas** `:0put=range(1,1000)`
- **Reemplazar palabras** `1,$s/lock/string/g`
- **Reemplazo de espacios a sangria** `=G` Permite corregir de espacio a sangria en todo el bloque o documento hacia abajo del cursor.
- **Usar vim en la consola** `set -o vi`
- **remueve los separadores** `ls | awk -F' ' '{print $4}'`

## Listar variable con número
i1 <Esc>
`Y999p` # Copia la linea y la pega 999 veces más
`VG` # Seleciona la linea y se va a la ultima línea.
`g<C-a>` # Seleciona en modo global para aplicar el efecto de autoincremento.

## Calculadora
1. **debes presionar** `Ctrl+r` (en modo inserción)
2. **Después presionar el (=) más  el valor y presionar enter**

## Como remover las ultimas caracteres

*primer método*

1.- `shift-A`
2.- `x`
3.- `.` (repite)

*segundo método*

1.- `/\.$` => borrara todos los puntos hasta el final

*tercer método*

1.- `:%s//`
2.- `:%s///`
3.- `*` // (buscara el ultimo palabra buscada )
4.-  `*`  %!xargs => buscara

## Filtrar datos con filtros en awk

- `:%awk -F'FOO' '{print $3}` **Esto permite mostrar filtrar y mostrar en el documento el resultado filtrado borrando el resto de datos del documento, FOO es el campo separador**
- `:%awk -F':' '{print $3}` **ejercicios**


