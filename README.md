# 🌿 EcoMarket — Calculadora de Huella de Carbono

Sitio web informativo y catálogo de productos para **EcoMarket**, una tienda de productos ecológicos, orgánicos y de residuo cero, que incluye una **calculadora de huella de carbono** para que los usuarios estimen su impacto ambiental mensual. El proyecto está construido **únicamente con HTML5 y CSS3**, sin JavaScript.

## ✨ Características

- **Home** (`index.html`): presentación de la empresa, su objetivo, su catálogo y su ética de trabajo.
- **Ofertas** (`views/ofertas.html`): productos en descuento, mostrando precio anterior, precio con oferta, nombre y porcentaje de descuento.
- **Productos** (`views/productos.html`): catálogo general de productos con nombre, precio e imagen.
- **Categorías** (`views/Categorias.html`): navegación por categorías de producto:
  - Aceites (`aceites.html`)
  - Cereales (`cereales.html`)
  - Condimentos (`condimentos.html`)
  - Cuidado personal (`cuidado_personal.html`)
  - Endulzantes (`endulzantes.html`)
  - Frutos secos (`frutos_secos.html`)
  - Harinas (`harinas.html`)
  - Limpieza (`limpieza.html`)
  - Nueces y semillas (`nueces_semillas.html`)
- **Calculadora de Huella de Carbono** (`views/calculadora.html`): formulario con el consumo de energía mensual del hogar, el medio de transporte principal y los kilómetros recorridos al mes; al marcar "Calcular Impacto Total" se revela un resultado estimado de emisiones (kg de CO₂ al mes), implementado sin JavaScript.
- **Contacto** (`views/contacto.html`): formas de contacto de la empresa (correo, teléfono, ubicación).
- **Comentarios** (`views/comentarios.html`): formulario para dejar nombre, correo, teléfono y comentario, con botón de reinicio y de envío (redirige al Home).
- **Sección de redes sociales**: enlaces a Facebook, Instagram y TikTok de EcoMarket, presente en el pie de página de todo el sitio.
- **Buscador**: campo de búsqueda visible en la barra de navegación (presente en todas las vistas).
- **Diseño responsivo**: la página se adapta a distintos tamaños de pantalla; las animaciones de entrada se desactivan en dispositivos móviles para evitar fallos de visualización.

> ⚠️ Nota: el resultado de la calculadora es un valor fijo de ejemplo (215 kg de CO₂ al mes) mostrado/ocultado mediante un `checkbox` y CSS; no se calcula dinámicamente a partir de los datos ingresados, ya que el proyecto no usa JavaScript.

## 🛠️ Tecnologías utilizadas

- **HTML5** — estructura semántica de todas las vistas.
- **CSS3** — estilos organizados en módulos:
  - `main.css` — estilos generales.
  - `layout.css` — estructura y disposición de la página.
  - `components.css` — estilos de componentes reutilizables, incluida la calculadora y su sección de resultado.
  - `animations.css` — animaciones de entrada, desactivadas en móvil.
- Sin JavaScript ni frameworks: la interactividad de la calculadora (mostrar/ocultar el resultado) se resuelve con el truco de `checkbox` + CSS (`:checked`).

## 📁 Estructura del proyecto

```
Proyecto_html_css-1/
├── index.html                  # Página principal (Home)
├── css/
│   ├── main.css                # Estilos generales
│   ├── layout.css              # Layout / estructura
│   ├── components.css          # Componentes reutilizables (incluye la calculadora)
│   └── animations.css          # Animaciones de entrada
├── views/
│   ├── Categorias.html         # Índice de categorías
│   ├── aceites.html
│   ├── cereales.html
│   ├── condimentos.html
│   ├── cuidado_personal.html
│   ├── endulzantes.html
│   ├── frutos_secos.html
│   ├── harinas.html
│   ├── limpieza.html
│   ├── nueces_semillas.html
│   ├── ofertas.html
│   ├── productos.html
│   ├── contacto.html
│   ├── comentarios.html
│   └── calculadora.html        # Calculadora de huella de carbono
└── img/                         # Imágenes del sitio y de los productos (img/productos/)
```

## 🚀 Instalación y visualización

Este proyecto es completamente estático (HTML + CSS), no requiere backend ni instalación de dependencias.

1. Clona el repositorio:
   ```bash
   git clone https://github.com/yondermaldonado/Examen-Final-Calculadora-de-Huella-de-Carbono.git
   cd "Examen-Final-Calculadora-de-Huella-de-Carbono/Proyecto_html_css-1"
   ```

2. Abre `index.html` directamente en tu navegador, o sírvelo con un servidor local (opcional):

   ```bash
   python3 -m http.server 8080
   ```

   y accede a `http://localhost:8080/index.html`.

3. Navega por el sitio usando el menú superior: Home, Ofertas, Productos, Categorías, Contacto, Comentario y Calculadora.

## 👤 Autor

Yonder Daniel Maldonado Pabón

## 📄 Licencia

Este proyecto se distribuye con fines educativos. Puedes usarlo y adaptarlo libremente citando la fuente.
