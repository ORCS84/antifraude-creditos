
# AntiFraude Créditos - COMPILACIÓN FÁCIL

## Opción 1: COMPILACIÓN AUTOMÁTICA (Recomendada - Sin instalar nada)

1. Crea un repo nuevo en GitHub.com (ej. antifraude-creditos)
2. Sube TODO el contenido de esta carpeta a ese repo
3. Ve a la pestaña Actions en GitHub
4. Verás que se está compilando solo -> espera 3-4 minutos
5. Al terminar, descarga el APK en Artifacts > antifraude-creditos-apk
6. ¡Listo! Ese app-debug.apk ya se instala en cualquier Android

## Opción 2: Compilación Local (Android Studio)

Requisitos: Node.js 18+, Android Studio, Java 17

```bash
npm install
npx cap add android
npx cap copy
npx cap open android
```

En Android Studio:
Build > Build APK(s)

El APK está en: android/app/build/outputs/apk/debug/app-debug.apk

## Opción 3: APK Firmado para Play Store

En Android Studio:
Build > Generate Signed Bundle / APK
- Crea nuevo keystore (guárdalo bien)
- Elige Android App Bundle (AAB)
- Build -> sube ese .aab a Play Console

## Estructura
- public/index.html = tu app completa
- public/icons/ = iconos 192 y 512
- capacitor.config.json = config

Package: com.antifraude.creditos
Nombre: AntiFraude Créditos
Color: #166534 verde confianza
