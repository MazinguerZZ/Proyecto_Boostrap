# Kylian Mbappé — Página de Fans

Proyecto de práctica con **Bootstrap 5** que consiste en una página web dedicada a Kylian Mbappé, con información biográfica, logros deportivos y una tienda con formulario de pedido.

---

## 📁 Estructura del proyecto

```
├── proyecto.html       # Página principal
├── formulario.html     # Tienda oficial / formulario de pedido
├── proyecto.css        # Estilos personalizados
└── imagenes/
    ├── presentacion.jpeg
    ├── logo mbappe.png
    ├── mbappe celebrando gol.webp
    ├── jugando.jpeg
    ├── copa.jpg
    ├── seleccion.jpg
    ├── camiseta.webp
    ├── zapatilla.png
    ├── balon.png
    └── figura.png
```

---

## 📄 Páginas

### `proyecto.html` — Página principal
- **Hero section** con imagen de fondo y llamada a la acción hacia la tienda.
- **Biografía** en layout de dos columnas (texto + imagen).
- **Logros y estadísticas** presentados en cards (títulos, goles y premios).
- **Galería** de imágenes de su carrera.
- **Banner CTA** con enlace directo a la tienda.

### `formulario.html` — Tienda oficial
- Catálogo de **4 productos** (camiseta, botas, balón firmado, figura coleccionable) con selección de cantidad y talla.
- Formulario de **información de envío** con validación HTML5.
- Sección de **método de pago** con tres opciones (tarjeta, PayPal, transferencia bancaria). Los campos de tarjeta se muestran u ocultan mediante CSS puro según la selección.
- Aviso de envío gratuito para pedidos superiores a 50 €.

---

## 🎨 Diseño y personalización

Los colores del proyecto están inspirados en la bandera francesa y los colores del Real Madrid:

| Variable | Color | Uso |
|---|---|---|
| Primario | `#0055A4` | Navbar, botones, textos destacados |
| Secundario | `#003cff` | Header de la tienda |
| Hover primario | `#003d7a` | Estado hover de botones |

Otras decisiones de diseño:
- **Fuente:** Segoe UI / Tahoma (pila sans-serif del sistema).
- **Cards** con efecto `translateY` al pasar el cursor.
- **Imágenes de producto** con altura fija (`550px` escritorio, `400px` móvil) y `object-fit: cover`.
- Mostrar/ocultar campos de pago implementado con el selector CSS `:checked ~ ` sin JavaScript.

---

## 🧩 Componentes de Bootstrap utilizados

- Sistema de **grid** (columnas responsivas en todas las secciones)
- **Navbar** fija con colapso en móvil
- **Cards** con imágenes
- **Forms** con validación (`needs-validation`)
- **Buttons** y **button groups** (selector de talla)
- **Alerts** informativos
- **List groups**
- **Badges** y utilidades de espaciado/color
- **Bootstrap Icons** (carrito, tarjeta, PayPal, banco)

---

## 🚀 Cómo ejecutar el proyecto

No se requiere ningún servidor ni instalación. Basta con abrir el archivo directamente en el navegador:

```bash
# Opción 1 — abrir directamente
Doble clic en proyecto.html

# Opción 2 — servidor local con VS Code
Instalar la extensión Live Server y pulsar "Go Live"

# Opción 3 — servidor local con Python
python -m http.server 8000
# Abrir http://localhost:8000/proyecto.html
```

> ⚠️ Las imágenes deben estar en la carpeta `imagenes/` junto a los archivos HTML para que se muestren correctamente.

---

## 📦 Dependencias externas (CDN)

| Librería | Versión | Uso |
|---|---|---|
| Bootstrap CSS | 5.3.5 | Framework de estilos y componentes |
| Bootstrap Icons | 1.11.1 | Iconografía (solo en formulario) |

No se utiliza JavaScript personalizado. Bootstrap JS se carga desde CDN únicamente para el colapso de la navbar.

---

## 📱 Responsive design

| Breakpoint | Cambios aplicados |
|---|---|
| `≥ 992px` (lg) | Layout de dos columnas en biografía y logros |
| `< 768px` (md) | Hero a 50vh, fuente de marca reducida, imágenes de card a 400px |

---

## ✍️ Autor

Práctica de Bootstrap — 2025  
Página de fans no oficial de Kylian Mbappé.
