# Modo Sustituir o Reemplaza

- **Buscar y reemplazar una palabra** `%s/origen/cambio/g`
- **Buscar y reemplazar** `%s/origen/cambio/gc`
- `DW`
- **Elimina una palabra y entra modo inserción** `cw`
- **Elimina la línea y entra modo inserción** `cc`
- **Elimina de la posición hacia final de la línea y entra modo inserción** `C`
- **podrá cambiar lo que esta adentro de un símbolo** `ci[símbolo]`

## Ejercicio
- **Reemplaza el patron por ejemplo "o" en las lineas** `:g/patron/normal ( @o | @q )`
- **Permite invertir de mayúsculas a minúsculas viceversa la línea** `g ~~`
- **comentar la línea usando el #** `:g/patron/s/#/g`
- **Cambiar lo que se encuentre en el paréntesis** `ci(`
- **cambiar las lineas de primera hasta el final del documento** `1,$s/lock/string/g`
