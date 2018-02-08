### git tag
Listar las etiquetas en orden alfabético.

### git tag -a nom_etiqueta -m mensaje_etiqueta
Etiqueta anotada. Se guarda en la base de datos de git como un objeto entero. Tiene un checksum y contiene el nombre del etiquetador, correo, electrónico y fecha; y un mensaje asociado.

```
$ git tag -l "v1.*"
```
Lista las etiquetas que coincidan con el patron especificado.
