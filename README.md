# Pumitas Arcade — proyecto Android

Frontend Android de estilo arcade para importar y organizar archivos ROM ZIP de Neo Geo y enviarlos a RetroArch con el núcleo FinalBurn Neo (FBNeo).

## Estado
Este repositorio contiene el código fuente y un flujo de compilación en GitHub Actions. **No incluye todavía un APK compilado** ni un motor de emulación integrado. La compilación requiere Android SDK y Gradle; este entorno de preparación no dispone de ellos.

## Compilar en GitHub
1. Crea un repositorio nuevo en GitHub.
2. Descomprime este proyecto y sube el contenido de la carpeta `pumitas_arcade` al repositorio (la carpeta `.github/workflows` debe quedar en la raíz).
3. Abre la pestaña **Actions** y ejecuta **Build Pumitas Arcade APK** (o espera a que termine el flujo al subir a `main`/`master`).
4. Cuando termine correctamente, abre la ejecución y descarga el artefacto `pumitas-arcade-debug-apk`.
5. Descomprime el artefacto y tendrás `app-debug.apk`, que podrás instalar en Android habilitando la instalación desde esa fuente.

## Requisitos para jugar
- Android 6.0 o posterior (arm64 recomendado).
- RetroArch Android de 64 bits instalado.
- Núcleo FinalBurn Neo (FBNeo) instalado en RetroArch.
- ROMs y BIOS Neo Geo compatibles, aportadas por el usuario y obtenidas legalmente. No se incluyen ROMs ni BIOS.

## Limitaciones de esta versión
- Es un frontend: no integra el núcleo FBNeo dentro del APK.
- La reproducción depende de RetroArch y de que la versión instalada acepte la actividad y los extras usados por la app.
- Los controles táctiles, guardado de estados y otras funciones avanzadas dependen de RetroArch.
