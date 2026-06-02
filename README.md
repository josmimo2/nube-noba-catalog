# Nube Noba — Catálogo Web 2025

Catálogo interactivo de pendientes artesanales para GitHub Pages.

## 🚀 Publicar en GitHub Pages

1. Crea un repositorio en GitHub (ej. `nube-noba-catalogo`)
2. Sube la carpeta completa (arrastra los archivos al repositorio)
3. Ve a **Settings → Pages → Branch: main → / (root)** → Guardar
4. En 1-2 minutos tu web estará en:
   `https://tuusuario.github.io/nube-noba-catalogo`

## 🖼️ Añadir fotos reales

Crea una carpeta `img/` y añade las fotos con estos nombres exactos:

```
img/pendiente-01.jpg   → Fantasmas
img/pendiente-02.jpg   → Dados
img/pendiente-03.jpg   → Corazones rosas
img/pendiente-04.jpg   → Corazones rojos
img/pendiente-05.jpg   → Fresas
img/pendiente-06.jpg   → TNT
img/pendiente-07.jpg   → Sandías
img/pendiente-08.jpg   → Bloques "?"
img/pendiente-09.jpg   → Sol
img/pendiente-10.jpg   → Cigarrillos
img/pendiente-11.jpg   → Huevos fritos
img/pendiente-12.jpg   → Cartas de amor
img/pendiente-13.jpg   → Carne y huesos
img/pendiente-14.jpg   → Ojos rojos
img/pendiente-15.jpg   → Sombrero de paja
img/pendiente-16.jpg   → Tierra
img/pendiente-17.jpg   → Cubos tierra
img/pendiente-18.jpg   → Cubos hielo
img/pendiente-19.jpg   → Nube y lluvia
img/pendiente-20.jpg   → Reflejos de agua
img/pendiente-21.jpg   → Jin y Jan
img/pendiente-22.jpg   → Ojos negros
img/pendiente-23.jpg   → Manolo
img/pendiente-24.jpg   → Slenderman
img/pendiente-25.jpg   → Bola de pinchos
img/pendiente-26.jpg   → Luna
img/pendiente-27.jpg   → Sobres sorpresa
```

Luego en `index.html`, en cada spread de producto, reemplaza el bloque `.photo-placeholder` por una etiqueta `<img>`:

```html
<!-- ANTES (placeholder) -->
<div class="photo-placeholder">
  <div class="photo-emoji">👻</div>
  ...
</div>

<!-- DESPUÉS (foto real) -->
<img src="img/pendiente-01.jpg" alt="Fantasmas" />
```

## ✏️ Editar productos

Los datos de los productos están en el array `products` al inicio del `<script>`:

```js
const products = [
  { name: 'Fantasmas', series: null, price: 3, emoji: '👻', desc: 'Descripción...' },
  ...
];
```

Cada campo:
- `name` — nombre del modelo
- `series` — serie (ej. `'Serie Minecraft'`) o `null`
- `price` — precio en euros
- `emoji` — emoji decorativo (se sustituirá por la foto)
- `desc` — descripción del producto

## 📱 Características

- ✅ Navegación con botones, teclado (← →) y swipe táctil
- ✅ Barra de progreso
- ✅ Índice clicable
- ✅ Responsive para móvil
- ✅ Sin dependencias externas (solo Google Fonts)
- ✅ Un único archivo HTML — fácil de editar
