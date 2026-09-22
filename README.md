# Pasito

**Diario personal para Windows. Escribe para ti.**

Pasito es una aplicación de escritorio pensada para escribir con libertad, mantener perfiles locales separados y guardar el contenido privado en el propio equipo.

> **Estado actual:** en desarrollo. Todavía no hay una versión pública para descargar.

## Qué busca Pasito

- Escritura personal sin cuentas obligatorias.
- Perfiles locales independientes.
- Datos privados almacenados en el equipo del usuario.
- Protección de escritos y configuración privada.
- Personalización de la experiencia.
- Actualizaciones oficiales verificadas antes de instalarse.

## Privacidad

Pasito está diseñado para funcionar de forma local. No necesita registrar correo, teléfono ni una cuenta en la nube para escribir.

Cuando exista distribución pública, la comprobación de actualizaciones consultará únicamente la infraestructura oficial de Pasito en GitHub para saber si hay una versión nueva. Esa comprobación no necesita enviar escritos, nombres de perfiles, fotos, contraseñas ni claves de recuperación.

Consulta [PRIVACY.md](PRIVACY.md) para más detalles.

## Actualizaciones oficiales

Las futuras versiones públicas de Pasito usarán un sistema de actualización con verificación criptográfica:

1. Pasito consulta la Release oficial.
2. Verifica la firma Ed25519 del manifiesto de actualización.
3. Comprueba tamaño y SHA-256 del instalador.
4. Rechaza una actualización si alguna verificación falla.
5. El usuario decide si desea instalarla.

Más información en [SECURITY.md](SECURITY.md).

## Descargas

Todavía no existe una Release pública estable.

Cuando haya una beta disponible, las descargas oficiales aparecerán únicamente en la sección **Releases** de este repositorio.

## Código fuente

Este repositorio público **no contiene el código fuente de Pasito**. Se utiliza para información pública, documentación, futuras Releases y distribución oficial.

El desarrollo interno se mantiene en un repositorio privado.

## Créditos

**PasitoPs** — dirección creativa, diseño y desarrollo.

**Xyam (Sam)** — identidad sonora.

## Estado del proyecto

La rama de desarrollo actual ha alcanzado la base de **v0.30**, incluyendo la infraestructura inicial para actualizaciones oficiales verificadas. La siguiente etapa es preparar el instalador de Windows y probar el flujo completo de actualización antes de publicar una beta.

---

**Pasito**  
_De a pasitos nos vamos entendiendo._
