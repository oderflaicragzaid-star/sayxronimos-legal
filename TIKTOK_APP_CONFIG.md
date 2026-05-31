# Configuración TikTok App Review — Sayxrosnimos

> Archivo de referencia para el portal TikTok for Developers.
> Actualizar aquí cuando cambien credenciales o URLs.

---

## 📋 DATOS BÁSICOS DEL APP

| Campo en el portal | Valor exacto a usar |
|---|---|
| **App name** | `Sayxrosnimos` |
| **App description** | `Sayxrosnimos publishes stoicism and psychology videos to TikTok. Creator uses OAuth to authorize the app to post content` |
| **Category** | Education |

---

## 🌐 URLS DEL SITIO WEB

| Campo | URL |
|---|---|
| **Website URL** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/` |
| **Privacy Policy** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/privacy-policy.html` |
| **Terms of Service** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/terms-of-service.html` |
| **Redirect URI (Sandbox)** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/callback.html` |
| **Redirect URI (Production)** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/callback.html` |

---

## 🔑 CREDENCIALES TIKTOK

| Variable | Valor |
|---|---|
| **Client Key (Sandbox)** | `sbawwqyhc4a8ldq8ma` |
| **Client Secret (Sandbox)** | `5jGSSAy5YBG5w3LrmywR6Hho7rKczlYH` |
| **Client Key (Production)** | `awafla4nobub07et` |
| **Client Secret (Production)** | `MhujUv67LK9mfCs6L2Rcihlu4YZMfTJH` |
| **TikTok Username** | `@sayxrosnimos5` |

---

## 🖼️ IMÁGENES

| Elemento | Ruta local |
|---|---|
| **Logo 1024×1024 (para portal TikTok)** | `C:\Users\Leidy\Documents\Alfredo\M_Youtube_TikTok\Sayxrosnimos-1024-1024.png` |
| **Logo en web (favicon + header)** | `C:\Users\Leidy\Documents\Alfredo\M_Youtube_TikTok\legal\logo.png` |

> ⚠️ Ambas son la misma imagen. En el portal TikTok subir `Sayxrosnimos-1024-1024.png`.

---

## 📁 REPOSITORIO GITHUB (legal pages)

| Elemento | Valor |
|---|---|
| **GitHub User** | `oderflaicragzaid-star` |
| **Repo name** | `sayxrosnimos-legal` |
| **Repo URL** | `https://github.com/oderflaicragzaid-star/sayxrosnimos-legal` |
| **GitHub Pages URL** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/` |
| **Token GitHub** | Ver git remote en carpeta `legal/` |
| **TikTok domain verify** | `tiktok6wENmkmEl57Ifl3rBG6Cw5RKfpKepzcf.txt` (ya subido) |

---

## 🔒 SCOPES SOLICITADOS

```
user.info.basic
video.publish
video.upload
```

---

## ✅ CHECKLIST PARA EL REVIEW

Antes de enviar a revisión, verificar:

- [ ] App name en portal = `Sayxrosnimos` (exactamente)
- [ ] Website URL en portal = `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/`
- [ ] Redirect URI en portal = `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/callback.html`
- [ ] Privacy Policy URL = `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/privacy-policy.html`
- [ ] Terms of Service URL = `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/terms-of-service.html`
- [ ] App icon subido = `Sayxrosnimos-1024-1024.png`
- [ ] El favicon aparece en el tab del navegador en las 3 páginas
- [ ] El logo aparece en el header de Privacy Policy y Terms of Service
- [ ] Existe botón "Login with TikTok" en la página principal

---

## 🗂️ ARCHIVOS LOCALES DEL SITIO LEGAL

```
legal/
├── index.html              ← Página principal con login button
├── privacy-policy.html     ← Política de privacidad
├── terms-of-service.html   ← Términos de servicio
├── callback.html           ← Página que recibe el código OAuth
├── logo.png                ← Logo (copia de Sayxrosnimos-1024-1024.png)
└── tiktok6wENmkmEl57...txt ← Verificación de dominio TikTok
```

---

## 📌 NOTAS IMPORTANTES

- **Ortografía correcta**: `Sayxros`**n**`imos` — con 's' antes de 'n'. **No** `Sayxronimos`.
- El repo GitHub se llamaba `sayxronimos-legal` (sin 's') — ya fue renombrado a `sayxrosnimos-legal`.
- La URL del portal de TikTok **debe actualizarse manualmente** para reflejar la nueva URL del repo.
- En el portal usar siempre el **Client Key de Producción** (`awafla4nobub07et`), no el de Sandbox.

---

*Última actualización: 2026-05-31*
