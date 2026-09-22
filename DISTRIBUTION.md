# Distribución oficial

Este repositorio será el punto público de distribución de Pasito.

## Canales previstos

### Estable

Versiones destinadas a uso normal.

Ejemplo:

```text
v1.0.0
v1.0.1
v1.1.0
```

### Beta

Versiones de prueba anteriores a una publicación estable. Pueden contener cambios todavía en validación.

## Contenido de una Release

Una Release oficial deberá contener como mínimo:

```text
Pasito_Setup_X.Y.Z.exe
update.json
update.sig
```

El instalador es el archivo que ejecuta el usuario.

`update.json` contiene los metadatos firmados de la versión.

`update.sig` permite que Pasito compruebe que el manifiesto fue autorizado por la clave oficial del proyecto.

## Regla de publicación

No se publicará una versión como estable hasta haber probado:

- instalación limpia;
- actualización desde una versión anterior;
- conservación de los datos locales;
- rechazo de una actualización manipulada;
- fallo de descarga;
- reinstalación;
- recuperación ante un error durante la actualización.

## Estado actual

Todavía no hay una descarga pública disponible.
