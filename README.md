# Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos

## Zonas de git
1.- Directorio de trabajo
2.- Area de preparación (staging área)
3.- Directorio Git (repositorio)

## Flujo de trabajo basico de Git.
1.- Modificas una serie de archivos en tu directorio de trabajo.
2.- Preparas los archivos añadiéndolos a tu área de preparación (staging área).
3.- Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

## Configurando Git por primera vez
Configura el nombre de usuario, correo y editor
```
git config --global user.name "Raúl Valdez Piedra"
git config --global user.email "rvaldez20@gmail.com"
git config --global core.editor opera
```

Consultar toda la configuración
```
git config --list
```

## Configuración de SSH en windows
1.- Creamos una carpeta llamada `llaves-ssh` en el disco `C:`para evitar problemas de ruta.
2.- Ejecutamos el comando `ssh-keygen -t rsa -C "mi-correo"`
El correo debe ser el mismo con el que se registro en github para evitar posibles problemas con rutas.
Dejamos el passphrase vacio y entre 2 veces.
3.- Iniciamos el ssh-agent en background ejecutabdo el comando  `eval "$(ssh-agent -s)"`
4.- Agregamos la lista ssh generada a ssh-agent ejecutando `ssh-add /c/llaves-ssh/github_rsa`
5.- DEsde ahora podemos hacer push y pull sin que github nos este pidiend el acceo.
