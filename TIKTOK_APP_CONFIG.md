# Configuración TikTok App Review — Sayxrosnimos

> Archivo de referencia completo para el portal TikTok for Developers.
> Usar como base al reconfigurar, crear una nueva app, o solucionar rechazos futuros.

---

## 📊 ESTADO ACTUAL

| Campo | Valor |
|---|---|
| **Estado** | 🟡 **In review** (enviado 2026-05-31) |
| **App ID** | `7639957495133308949` |
| **URL del app en portal** | https://developers.tiktok.com/app/7639957495133308949/pending |

---

## 📋 DATOS BÁSICOS DEL APP

| Campo en el portal | Valor exacto |
|---|---|
| **App name** | `Sayxrosnimos` |
| **Category** | `Education` |
| **App description (portal público, 120 chars)** | `Sayxrosnimos publishes stoicism and psychology videos to TikTok. Creator uses OAuth to authorize the app to post content` |
| **Platforms** | ✅ Web, ✅ Desktop |

> ⚠️ **ORTOGRAFÍA CRÍTICA**: El nombre es `Sayxros`**`n`**`imos` — con 's' antes de 'n'.
> Error histórico: se escribía `Sayxronimos` (sin 's') — causó 2 rechazos.

---

## 🌐 URLS DEL SITIO WEB (todas verificadas ✅)

| Campo en el portal | URL exacta |
|---|---|
| **Website URL** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/` |
| **Terms of Service URL** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/terms-of-service.html` |
| **Privacy Policy URL** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/privacy-policy.html` |
| **Redirect URI (Login Kit - Web)** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/callback.html` |
| **Redirect URI (Login Kit - Desktop)** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/callback.html` |

---

## 🔑 CREDENCIALES TIKTOK

| Variable | Valor | Entorno |
|---|---|---|
| **Client Key** | `sbawwqyhc4a8ldq8ma` | Sandbox |
| **Client Secret** | `5jGSSAy5YBG5w3LrmywR6Hho7rKczlYH` | Sandbox |
| **Client Key** | `awafla4nobub07et` | **Producción** ← usar en HTML |
| **Client Secret** | `MhujUv67LK9mfCs6L2Rcihlu4YZMfTJH` | Producción |
| **TikTok Username** | `@sayxrosnimos5` | — |
| **App ID** | `7639957495133308949` | — |

> ⚠️ En el HTML (`index.html`) usar siempre el **Client Key de Producción** (`awafla4nobub07et`), no el de Sandbox.
> Las credenciales completas también están en `.env` del proyecto.

---

## 🔒 PRODUCTS Y SCOPES

| Producto | Scopes | Uso |
|---|---|---|
| **Login Kit** | `user.info.basic` | Verificar identidad de la cuenta creadora |
| **Content Posting API** | `video.publish`, `video.upload` | Publicar videos educativos |

**Direct Post**: ✅ Habilitado (permite publicar directamente sin aprobación del usuario)

---

## 🖼️ IMÁGENES

| Elemento | Ruta local |
|---|---|
| **Logo 1024×1024 (subir al portal TikTok)** | `C:\Users\Leidy\Documents\Alfredo\M_Youtube_TikTok\Sayxrosnimos-1024-1024.png` |
| **Logo en web (favicon + header)** | `C:\Users\Leidy\Documents\Alfredo\M_Youtube_TikTok\legal\logo.png` |

> Ambas son la misma imagen. Al volver a Draft, el portal borra el icono — hay que re-subirlo manualmente.

---

## 📁 REPOSITORIO GITHUB

| Elemento | Valor |
|---|---|
| **GitHub User** | `oderflaicragzaid-star` |
| **Repo name** | `sayxrosnimos-legal` |
| **Repo URL** | `https://github.com/oderflaicragzaid-star/sayxrosnimos-legal` |
| **GitHub Pages URL base** | `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/` |
| **Token (en git remote)** | Ver: `git remote -v` dentro de la carpeta `legal/` |
| **Rama principal** | `main` |

### Archivos en el repo:

```
legal/
├── index.html                              ← Página principal con Login with TikTok
├── privacy-policy.html                     ← Política de privacidad
├── terms-of-service.html                   ← Términos de servicio
├── callback.html                           ← Recibe el código OAuth de TikTok
├── logo.png                                ← Logo (= Sayxrosnimos-1024-1024.png)
├── tiktok6wENmkmEl57Ifl3rBG6Cw5RKfpKepzcf.txt   ← Verificación dominio (1ra solicitud)
├── tiktok1j4NHhg84W4zzDGVY3qIWi10uJXZErY7.txt   ← Verificación dominio (2da solicitud)
└── TIKTOK_APP_CONFIG.md                    ← Este archivo
```

### Comandos git:
```bash
cd "C:\Users\Leidy\Documents\Alfredo\M_Youtube_TikTok\legal"
git add .
git commit -m "descripción del cambio"
git push origin main
```

---

## 🔐 VERIFICACIÓN DE DOMINIO (URL prefix)

TikTok requiere verificar que eres dueño del dominio/URL. Método usado: **URL prefix + signature file**.

| # Intento | Archivo de verificación | Estado |
|---|---|---|
| 1ra solicitud | `tiktok6wENmkmEl57Ifl3rBG6Cw5RKfpKepzcf.txt` | Eliminado del portal (era para URL vieja) |
| 2da solicitud | `tiktok1j4NHhg84W4zzDGVY3qIWi10uJXZErY7.txt` | ✅ **Activo y verificado** |

> Cada vez que cambies la URL del repo, TikTok genera un nuevo archivo de verificación.
> Pasos: portal → URL properties → Verify properties → URL prefix → descargar archivo → subir al repo → push → click Verify.

---

## 📝 DESCRIPCIÓN PARA EL APP REVIEW (campo largo, 1000 chars)

```
Sayxrosnimos is an automated content creation app that generates and publishes short educational videos about stoicism and psychology to TikTok. The app is used exclusively by the creator account @sayxrosnimos5.

Login Kit (user.info.basic): Used to authenticate and verify the connected TikTok creator account before posting. Only the open_id and display name are accessed to confirm account identity.

Content Posting API (video.publish, video.upload): Used to upload pre-generated educational video files to the authenticated TikTok creator account. Videos are created locally using text-to-speech, stock footage from Pexels, and FFmpeg. No user data is collected or stored externally.
```

> Para revisiones posteriores, agregar al final:
> `Changes in this revision: [describir qué cambió]`

---

## ✅ CHECKLIST COMPLETO PARA EL REVIEW

### Antes de hacer "Submit for review":

**App details:**
- [ ] App name = `Sayxrosnimos` (verificar ortografía, especialmente la 's' antes de 'n')
- [ ] App icon subido (1024×1024px) = `Sayxrosnimos-1024-1024.png`
- [ ] Category = `Education`
- [ ] App description (120 chars) correcta y sin caracteres especiales
- [ ] Terms of Service URL con `sayxrosnimos-legal` (con 's')
- [ ] Privacy Policy URL con `sayxrosnimos-legal` (con 's')
- [ ] Platforms: Web ✅ y Desktop ✅
- [ ] Web/Desktop URL = `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/`
- [ ] URL prefix verificada en "URL properties" (sin errores rojos)

**Products:**
- [ ] Login Kit: Redirect URI = `https://oderflaicragzaid-star.github.io/sayxrosnimos-legal/callback.html`
- [ ] Content Posting API activo con Direct Post habilitado

**App review:**
- [ ] Descripción de productos/scopes completa (ver sección arriba)
- [ ] Video demo subido (formato mp4/mov, máx 50MB)
- [ ] Motivo del submit completado (máx 120 chars)

**Sitio web (GitHub Pages):**
- [ ] `index.html`: tiene botón "Login with TikTok" visible
- [ ] `index.html`: título `<title>Sayxrosnimos — Stoic Content Creator</title>`
- [ ] `privacy-policy.html`: tiene favicon + logo en header + menciona "Sayxrosnimos"
- [ ] `terms-of-service.html`: tiene favicon + logo en header + menciona "Sayxrosnimos"
- [ ] Logo aparece en la pestaña del navegador (favicon) en las 3 páginas
- [ ] Archivo de verificación TikTok presente en el repo

---

## 🔄 PROCESO PASO A PASO PARA NUEVA SOLICITUD

### Si necesitas crear una nueva app desde cero:

1. Ir a https://developers.tiktok.com/apps/ → `+ Connect an app`
2. Completar App name = `Sayxrosnimos`, Category = Education
3. Subir logo `Sayxrosnimos-1024-1024.png`
4. Completar description (120 chars, sin caracteres especiales)
5. Terms of Service URL + Privacy Policy URL (ver sección URLs)
6. Platforms: Web + Desktop
7. Web/Desktop URL
8. Ir a **URL properties** → Verify properties → URL prefix → descargar archivo → subirlo al repo → push → Verify
9. En Products: agregar Login Kit + Content Posting API
10. Redirect URI en Login Kit
11. Ir a **App review** → completar descripción larga + subir video demo
12. Submit for review → escribir motivo

### Si el review fue rechazado:

1. Leer el mensaje exacto del reviewer
2. `Return to Draft` → Confirm
3. Re-subir el app icon (siempre se borra)
4. Hacer los cambios indicados
5. Si cambiaste URLs: re-verificar el dominio (URL properties)
6. `Submit for review` → escribir nuevo motivo explicando los cambios

---

## 📚 HISTORIAL DE RECHAZOS Y SOLUCIONES

### Rechazo #1 (mayo 2026)
**Motivos:**
- App icon no aparecía en PP/ToS (faltaba favicon y logo en header)
- App name diferente al de la web ("EstoicismoBot" en portal vs "Sayxronimos" en web)
- PP no mencionaba el app por nombre
- ToS no mencionaba el app por nombre
- Sin login entry point en el website
- El icono del portal no coincidía con el de la web

**Solución:**
- Se creó sitio web completo en GitHub Pages (`legal/`) con PP, ToS, login button
- Se cambió nombre en portal a `Sayxrosnimos`
- Se actualizaron todos los archivos HTML con logo, favicon y nombre correcto

### Rechazo #2 (mayo 2026)
**Motivo:** "The app name and website title do not match the website URL"

**Causa raíz:** El repo GitHub se llamaba `sayxronimos-legal` (sin 's') pero el app name era `Sayxrosnimos` (con 's').

**Solución:**
- Repo renombrado vía GitHub API: `sayxronimos-legal` → `sayxrosnimos-legal`
- Todos los archivos HTML actualizados con la nueva URL
- Nuevo archivo de verificación de dominio generado y subido
- Redirect URI y todos los campos del portal actualizados
- Re-enviado a revisión (estado actual: **In review**)

---

## 🚨 ERRORES COMUNES A EVITAR

| Error | Solución |
|---|---|
| Escribir `Sayxronimos` (sin 's') | Siempre `Sayxros`**`n`**`imos` |
| App icon se borra al hacer "Return to Draft" | Re-subirlo manualmente cada vez |
| Description del portal tiene caracteres especiales | Usar solo ASCII básico, sin tildes ni símbolos |
| URL prefix no verificada → formulario no guarda | Verificar dominio antes de hacer submit |
| execCommand del diálogo de submit va al campo incorrecto | Hacer clic dentro del textarea del modal primero |
| Texto de App review muy largo (>1000 chars) | Truncar, límite estricto |
| Repo renombrado pero archivos HTML tienen URL vieja | Buscar con grep `sayxronimos-legal` en todos los .html y .py |

---

*Última actualización: 2026-05-31 — Sesión de corrección de URL mismatch y 2do submit a revisión*
