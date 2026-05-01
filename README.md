# 🛍️ PWA Emprendedor — Un Solo Producto
**Desarrollada por Vibras Positivas HM**

---

## ⚡ Archivos incluidos
| Archivo | Función |
|---|---|
| `index.html` | App completa (todo el código) |
| `sw.js` | Service Worker (modo offline) |
| `manifest.json` | Metadatos PWA (instalación) |

---

## 🎨 PERSONALIZACIÓN (5 minutos)

Abre `index.html` y busca el objeto `CONFIG` (línea ~350):

```javascript
const CONFIG = {
  negocio: "Doña Carmen",          // ← Nombre del negocio
  producto: "Arepa con Queso",     // ← Nombre del producto
  descripcion: "Descripción...",   // ← Descripción corta
  precio: 8500,                    // ← Precio en números (sin $ ni puntos)
  moneda: "$",                     // ← Símbolo de moneda
  separadorMiles: ".",
  emoji: "🫓",                     // ← Emoji del producto (si no hay imagen)
  imagenUrl: "",                   // ← URL de imagen (opcional)
  whatsappNumero: "573117700431",  // ← Tu número con código de país (sin +)
  whatsappPrefijo: "¡Hola! Quiero hacer un pedido 🛒",
};
```

### Cambiar imagen del producto
- Sube tu foto a Cloudinary, ImgBB o similar
- Pega la URL en `imagenUrl: "https://..."`
- El emoji se reemplaza automáticamente por la imagen

---

## 🚀 DESPLIEGUE EN GITHUB PAGES

1. Crea repo en GitHub (ej: `arepa-pedidos`)
2. Sube los 3 archivos: `index.html`, `sw.js`, `manifest.json`
3. Ve a Settings → Pages → Source: main / root
4. Tu app estará en: `https://tuusuario.github.io/arepa-pedidos`

## 🌐 DESPLIEGUE EN NETLIFY (recomendado para PWA)
1. Arrastra la carpeta a netlify.com/drop
2. URL instantánea tipo `https://random-name.netlify.app`
3. Cambia el dominio en Site Settings

---

## 📱 CÓMO INSTALAR EN CELULAR (el cliente)

### Android (Chrome):
- Abrir la URL en Chrome
- Menú (3 puntos) → "Añadir a pantalla de inicio"
- O esperar el banner automático de instalación

### iPhone (Safari):
- Abrir la URL en Safari (¡no Chrome!)
- Botón Compartir → "Añadir a inicio"

---

## ✅ FUNCIONALIDADES
- ✅ Pantalla producto con animación flotante
- ✅ Un toque → formulario de pedido
- ✅ Selector de cantidad con total automático
- ✅ Datos guardados en localStorage (no vuelven a escribir)
- ✅ GPS para capturar ubicación exacta (Google Maps link)
- ✅ Envío por WhatsApp con mensaje formateado
- ✅ Instalar como app (PWA)
- ✅ Funciona offline (service worker)
- ✅ Habeas Data (Ley 1581/2012)
- ✅ Footer Vibras Positivas HM

---

## 💬 Mensaje WhatsApp generado (ejemplo):
```
¡Hola! Quiero hacer un pedido 🛒

🛍️ PRODUCTO: Arepa con Queso Especial
🔢 CANTIDAD: 2
💰 TOTAL: $17.000

👤 NOMBRE: María García
📍 DIRECCIÓN: Cll 20 #15-30, Barrio Centro
📱 CELULAR: 3001234567
💬 WHATSAPP: 3001234567
📝 OBSERVACIONES: Sin sal extra

📌 UBICACIÓN GPS:
https://www.google.com/maps?q=8.123456,-75.654321

_Pedido enviado desde la app_
```

---

**Vibras Positivas HM — haroldco45@gmail.com — 3117700431**
