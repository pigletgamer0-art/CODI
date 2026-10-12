# CODI · Compilación Android

Este repositorio está preparado para compilar **CODI Academy CrashFix** desde el código Java completo mediante GitHub Actions.

## Subir el proyecto

1. Descarga `CODI-Android-Source-Para-GitHub.zip` desde la conversación de ChatGPT.
2. En este repositorio abre **Add file → Upload files**.
3. Sube el **ZIP sin descomprimir** y conserva exactamente el nombre `CODI-Android-Source-Para-GitHub.zip`. Si Chrome lo renombra, cámbialo antes de subir.
4. Pulsa **Commit changes** en `main`.
5. En **Actions → Compilar CODI Android → Run workflow** puedes iniciar la compilación; si GitHub Actions está habilitado, la subida del ZIP también la inicia automáticamente.
6. Tras aparecer una ejecución con marca verde, ábrela y descarga **CODI-Android-Debug-APK** desde *Artifacts*. Descomprime el ZIP de artifacto para obtener `app-debug.apk`.

## Avisos

- El APK nuevo es **una beta de prueba**: aún se debe validar en un teléfono físico.
- Package ID: `cl.codi.academy.crashfix`; no reemplaza a las betas viejas ni migra datos de ellas automáticamente.
- Para instalación, revisa previamente que los permisos sean correctos y que el APK proceda de una compilación propia.
- Las cuentas remotas no estarán activas hasta publicar el backend HTTPS correspondiente.
- No subas contraseñas ni claves de firma al repositorio.

La configuración de compilación está en `.github/workflows/build-codi.yml`.
