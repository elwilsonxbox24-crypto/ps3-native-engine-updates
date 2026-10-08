# PS3 Native Engine — Updates

Canal público de distribución del launcher para Windows 11. El código de desarrollo permanece en un repositorio privado.

**Estado:** aún no hay una versión publicada en GitHub Releases. Tener este repositorio creado no activa las descargas automáticamente.

## Canal Alpha

- Etiqueta de release: `channel-alpha`
- Archivo de control: `manifest.json`
- Firma del manifiesto: `manifest.json.sig` (RSA-PSS + SHA-256)
- Ejecutable: `Launcher-<versión>.exe`, con hash SHA-256 incluido en el manifiesto.
- URL que consulta el launcher: https://github.com/elwilsonxbox24-crypto/ps3-native-engine-updates/releases/download/channel-alpha/manifest.json

Las firmas se generan en la PC del desarrollador. **Nunca subir** `release-private.pem`, credenciales, juegos, firmware, archivos personales ni carpetas de desarrollo. La clave pública está integrada en el launcher para verificar la identidad del emisor.

### Publicación

Se prepara y firma la versión en la PC de desarrollo. Tras comprobar el ejecutable y verificar el manifiesto localmente, se suben únicamente el ejecutable, `manifest.json.sig` y `manifest.json` a una release `channel-alpha`, preferentemente cargando el manifiesto al final. Las descargas no deben ofrecerse hasta completar la prueba de actualización desde Windows.

PS3 Native Engine está en fase de launcher; todavía no ejecuta juegos de PS3.
