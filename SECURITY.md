# Seguridad de Pasito

Este documento describe el modelo de seguridad previsto para la distribución oficial de Pasito.

## Actualizaciones

Pasito no debe confiar en una actualización solamente porque provenga de GitHub.

Cada Release oficial deberá incluir:

```text
Pasito_Setup_X.Y.Z.exe
update.json
update.sig
```

El flujo de verificación previsto es:

1. obtener la información de la Release oficial;
2. verificar la firma Ed25519 de `update.json`;
3. comprobar que el manifiesto corresponde a Pasito y al canal correcto;
4. comprobar nombre, tamaño y SHA-256 del instalador;
5. aceptar descargas únicamente desde hosts HTTPS permitidos;
6. bloquear la actualización si falla cualquier comprobación;
7. pedir confirmación al usuario antes de abrir el instalador.

## Claves de firma

La clave privada que autoriza las actualizaciones oficiales:

- se genera fuera del repositorio público;
- está protegida con contraseña;
- no forma parte del ejecutable;
- no se publica en GitHub;
- no se distribuye con Pasito.

La aplicación incorpora únicamente la clave pública necesaria para verificar firmas.

## Datos del usuario

Los datos privados de cada instalación se crean en el equipo de esa persona. El instalador público no debe contener perfiles, escritos, respaldos, claves de recuperación ni datos del computador de desarrollo.

Antes de cada publicación se debe revisar el paquete final para impedir que archivos privados entren accidentalmente en una Release.

## Código fuente

El código fuente principal de Pasito no se distribuye desde este repositorio público.

## Reporte responsable

Si detectas una vulnerabilidad, evita publicar contraseñas, escritos, claves privadas o información personal en un Issue público. Utiliza un canal privado de contacto con el creador cuando el problema pueda exponer datos sensibles.
