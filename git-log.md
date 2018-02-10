# git log
Muestra todo el historial de commits del proyecto.

`$ git log --pretty=format:"%h - %an, %ar : %s"`
Muestra el historial con el formato que indicamos.

## Limitar la salida del historial
`$ git log -n`: Cambiamos la n por cualquier número entero, por ejemplo:
`$ git log -2`: Nos mostrará los 2 commits más recientes.

`$ git log --after="2018/02/08 00:00:00"`: Muestra los commits relizados despues de la fecha y hora especificada.
`$ git log --before="2018/02/08 00:00:00"`: Muestra los commits realizados antes de la fecha y hora especificada.

Las banderas del comando `git log` se pueden usar juntas según convenga, por ejemplo:
`$ git log --after="2018/02/07 00:00:00" --before="2018/02/08 00:00:00"`

`$ git log --decorate --oneline --all --graph`
Este comando nos muestra el historial en una sola línea por commit y ademas muestra todos los commits y mueestra las ramificaciones.

`$ git log --oneline `
Este comando nos muestra el historial en una sola línea por commit.
