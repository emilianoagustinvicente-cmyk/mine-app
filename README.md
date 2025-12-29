 🚜 MineFleet: Manual de Despliegue y APK

Este documento detalla los pasos para poner tu aplicación en línea y transformarla en una APK de Android.

## 1️⃣ Alojar el código en GitHub
1. **Crear Repositorio**: Ve a [GitHub](https://github.com/new) y crea uno llamado `minefleet`.
2. **Subir Archivos**: Usa la opción "uploading an existing file" y arrastra todos los archivos de esta carpeta.
3. **Commit**: Haz clic en "Commit changes" para guardar.

## 2️⃣ Poner la App en línea (Hosting)
Para generar la APK, la app necesita una URL pública (HTTPS).
### Recomendación: Vercel (Gratis y Rápido)
1. Crea cuenta en [Vercel.com](https://vercel.com/) usando tu GitHub.
2. Haz clic en **"Import"** sobre tu repositorio `minefleet`.
3. Haz clic en **"Deploy"**.
4. Copia la URL que te entreguen (ej: `https://minefleet.vercel.app`).

## 3️⃣ Generar la APK (Android)
1. Ve a [PWABuilder.com](https://www.pwabuilder.com/).
2. Pega la URL de tu app (la de Vercel).
3. Haz clic en **"Build My App"**.
4. Descarga el paquete de **Android**.
5. Dentro del ZIP, encontrarás el archivo `.apk` para instalar en cualquier teléfono.

## 📡 Uso en la Mina (Modo Offline)
La aplicación está configurada con un **Service Worker**. Esto significa que:
- La primera vez que abras la app con internet (o la APK), se descargará internamente.
- Las siguientes veces podrás abrirla **sin señal de celular**.
- Los datos se guardan en el teléfono y se mantienen aunque cierres la app.

---
