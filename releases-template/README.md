# Plantilla para el repositorio de releases (sin código fuente)

Copia estos archivos a un repositorio **separado** (por ejemplo `Anisphere-releases`).

## Contenido recomendado del repo

- `update.json` — fuente de verdad para la app
- `README.md` — notas para usuarios
- APKs publicados solo como **GitHub Releases** (assets), no hace falta subir el código de Anisphere

## Flujo al publicar una nueva versión

1. Sube el APK a un GitHub Release (el nombre del release puede ser cualquiera).
2. Calcula el SHA-256 del APK:

```bash
# Windows PowerShell
Get-FileHash .\anisphere-0.0.2.apk -Algorithm SHA256

# macOS / Linux
shasum -a 256 anisphere-0.0.2.apk
```

3. Actualiza `update.json` en la rama `main` (raw URL HTTPS):

```json
{
  "version": "0.0.2",
  "versionCode": 2,
  "releaseName": "Anisphere Beta 0.0.2",
  "channel": "beta",
  "downloadUrl": "https://github.com/OWNER/Anisphere-releases/releases/download/TAG/anisphere-0.0.2.apk",
  "sha256": "abc123...",
  "minimumAndroid": 7,
  "mandatory": false,
  "publishedAt": "2026-08-10",
  "changelog": ["…"]
}
```

4. En el proyecto de la app, configura:

```text
EXPO_PUBLIC_UPDATE_MANIFEST_URL=https://raw.githubusercontent.com/OWNER/Anisphere-releases/main/update.json
```

o edita `src/updates/config.ts`.

## Reglas

- `versionCode` debe subir siempre (1, 2, 3…).
- No uses el título del GitHub Release como fuente de verdad.
- Solo HTTPS.
- La app compara `versionCode` e ignora downgrades.
