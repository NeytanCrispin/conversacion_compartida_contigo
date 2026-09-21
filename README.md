# 🌻 Página Web de Flores Amarillas — 21 de Septiembre

Una página web interactiva y romántica creada para sorprender a tu pareja el **21 de septiembre**, el tradicional Día de las Flores Amarillas. Incluye animaciones, una carta secreta y una lluvia constante de pétalos y destellos, todo en un **único archivo HTML** sin dependencias externas más allá de una fuente de Google Fonts.

---

## 📋 Descripción General

Este proyecto consiste en una página web de una sola vista que muestra:

- Un **girasol animado dibujado íntegramente con CSS** (sin imágenes).
- Una **carta de amor oculta** que se revela al pulsar un botón.
- Una **lluvia continua de pétalos y destellos** con emojis animados.
- Un diseño cálido en tonos amarillos, crema y dorados.

El objetivo es ofrecer un detalle digital personalizado, fácil de enviar por WhatsApp, correo o mediante un enlace web público.

---

## 🛠️ Tecnologías y Lenguajes Necesarios

Solo se requieren **tres tecnologías estándar** que se integran en un único archivo:

| Tecnología | Función |
|------------|---------|
| **HTML** | Define la estructura: textos, contenedores, botón, carta y etiquetas. |
| **CSS** | Aporta el diseño, colores, tipografías y animaciones (pétalos cayendo, giro del girasol, transiciones). |
| **JavaScript** | Controla la interactividad: abrir la carta, generar la lluvia de pétalos y las ráfagas festivas. |

Además, se utiliza una fuente externa de **Google Fonts** (`Caveat` y `Montserrat`) para dar un estilo caligráfico y moderno.

---

## 📁 Estructura del Proyecto

```
flores-amarillas/
│
├── index.html      # Archivo único con HTML, CSS y JS integrados
└── README.md       # Este documento
```

---

## 🚀 Guía de Uso Paso a Paso

### Paso 1: Crear el archivo

1. Abre un editor de texto (Bloc de Notas, VS Code, Sublime Text, etc.).
2. Copia el código completo proporcionado en la sección [Código Completo](#-código-completo).
3. Guarda el archivo exactamente con el nombre:

   ```
   index.html
   ```

> ⚠️ Asegúrate de que la extensión sea `.html` y no `.txt`.

### Paso 2: Personalizar el mensaje

Abre `index.html` y modifica las siguientes secciones:

#### a) Dedicatoria de la carta

Busca dentro del `<div class="letter-content">` y reemplaza el texto por tu mensaje personal:

```html
<div class="letter-content">
  Hoy inicia la primavera y no podía dejar pasar este 21 de septiembre
  sin recordarte lo importante que eres para mí.

  Estas flores nunca se marchitarán, al igual que todo el cariño
  y la felicidad que traes a mis días.
</div>
```

#### b) Firma

Cambia la firma por tu nombre o apodo cariñoso:

```html
<div class="letter-signature">— Con todo mi amor 💛</div>
```

#### c) (Opcional) Título y etiqueta

Puedes personalizar:

- `<div class="date-tag">21 de Septiembre 🌼</div>`
- `<h1>¡Feliz Día de las Flores Amarillas!</h1>`

### Paso 3: Publicarlo gratis y compartirlo

#### Opción 1 — Netlify Drop (la más fácil, ~10 segundos)

1. Coloca `index.html` dentro de una carpeta.
2. Entra a [app.netlify.com/drop](https://app.netlify.com/drop).
3. Arrastra la carpeta a la página.
4. Obtendrás un enlace público tipo `https://flores-amarillas-xxx.netlify.app`.
5. Envíalo por WhatsApp.

#### Opción 2 — Vercel

1. Entra a [vercel.com](https://vercel.com).
2. Arrastra la carpeta con `index.html`.
3. Obtienes tu URL lista en ~30 segundos.

#### Opción 3 — GitHub Pages

1. Sube `index.html` a un repositorio público.
2. Activa **Pages** en la configuración del repositorio.
3. Accede al enlace generado.

#### Opción 4 — Envío directo por WhatsApp/Telegram

1. Adjunta el archivo `index.html` directamente en el chat.
2. Ella lo descarga, lo abre y su navegador (Chrome/Safari) lo mostrará automáticamente.

---

## 🎨 ¿Qué Muestra el Código?

### 1. Fondo con degradado cálido
Degradado radial en tonos crema y amarillo suave (`#fff9e6` → `#ffe082`).

### 2. Lluvia continua de flores y destellos
Caída infinita de emojis (`🌻`, `🌼`, `💛`, `✨`, `🌸`) con rotación, diferentes tamaños, velocidades y transparencias.

### 3. Tarjeta central decorativa
Recuadro blanco translúcido con bordes redondeados, sombra suave y borde dorado que contiene:

- Etiqueta superior: **"21 de Septiembre 🌼"**
- Título principal: **"¡Feliz Día de las Flores Amarillas!"**
- **Girasol animado en CSS**: centro marrón con 12 pétalos amarillos que giran lentamente y flotan.
- Texto introductorio sobre el significado de regalar flores amarillas.
- Botón dorado: **"Toca para abrir tu carta ✨"**

### 4. Carta oculta revelada
Al pulsar el botón:

- El botón desaparece.
- Se lanza una **ráfaga rápida de 28 pétalos**.
- Se despliega un recuadro amarillo simulando una carta escrita a mano (tipografía `Caveat`).
- Muestra la dedicatoria personalizada y la firma.

---

## ✨ Características Técnicas

| Característica | Detalle |
|----------------|---------|
| **Archivo único** | Todo el HTML, CSS y JS está integrado en `index.html`. |
| **Sin imágenes externas** | El girasol está dibujado con CSS puro. |
| **Responsive** | Se adapta a móviles y escritorio gracias al `viewport` y anchos relativos. |
| **Animaciones CSS** | `floatFlower`, `spinRays`, `fallDown`, `fadeIn`, `popLetter`. |
| **Animaciones JS** | Generación dinámica de pétalos con `setInterval` y `setTimeout`. |
| **Tipografías** | `Caveat` (carta) y `Montserrat` (interfaz) desde Google Fonts. |

---

## 🧩 Código Completo

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>21 de Septiembre 🌻</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@600&family=Montserrat:wght@400;600&display=swap" rel="stylesheet">

  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      min-height: 100vh;
      background: radial-gradient(circle at center, #fff9e6 0%, #ffe082 100%);
      font-family: 'Montserrat', sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      overflow-x: hidden;
      color: #4a2c00;
      padding: 20px;
    }

    .main-card {
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(8px);
      padding: 30px 25px;
      border-radius: 28px;
      box-shadow: 0 15px 35px rgba(212, 160, 23, 0.25);
      text-align: center;
      max-width: 440px;
      width: 100%;
      position: relative;
      z-index: 10;
      border: 2px solid rgba(255, 213, 79, 0.6);
      animation: fadeIn 1.2s ease-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    .date-tag {
      display: inline-block;
      background: #fff3e0;
      color: #e65100;
      padding: 6px 16px;
      border-radius: 20px;
      font-size: 0.85rem;
      font-weight: 600;
      letter-spacing: 1px;
      text-transform: uppercase;
      margin-bottom: 12px;
    }

    h1 {
      font-size: 1.8rem;
      color: #d84315;
      margin-bottom: 10px;
      line-height: 1.3;
    }

    .sunflower-wrap {
      width: 130px;
      height: 130px;
      margin: 15px auto;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      animation: floatFlower 3s ease-in-out infinite;
    }

    @keyframes floatFlower {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50%      { transform: translateY(-8px) rotate(4deg); }
    }

    .center-flower {
      width: 46px;
      height: 46px;
      background: radial-gradient(circle, #5d4037 30%, #3e2723 100%);
      border-radius: 50%;
      z-index: 3;
      box-shadow: inset 0 0 6px rgba(0,0,0,0.4);
    }

    .petals-ring {
      position: absolute;
      width: 100%;
      height: 100%;
      animation: spinRays 25s linear infinite;
    }

    @keyframes spinRays { 100% { transform: rotate(360deg); } }

    .petal-leaf {
      position: absolute;
      top: 50%;
      left: 50%;
      width: 18px;
      height: 60px;
      background: linear-gradient(to top, #ffca28, #fdd835, #fff176);
      border-radius: 50% 50% 20% 20%;
      transform-origin: 50% 0%;
      box-shadow: 0 0 4px rgba(255, 179, 0, 0.4);
    }

    .p1  { transform: translate(-50%, 0) rotate(0deg); }
    .p2  { transform: translate(-50%, 0) rotate(30deg); }
    .p3  { transform: translate(-50%, 0) rotate(60deg); }
    .p4  { transform: translate(-50%, 0) rotate(90deg); }
    .p5  { transform: translate(-50%, 0) rotate(120deg); }
    .p6  { transform: translate(-50%, 0) rotate(150deg); }
    .p7  { transform: translate(-50%, 0) rotate(180deg); }
    .p8  { transform: translate(-50%, 0) rotate(210deg); }
    .p9  { transform: translate(-50%, 0) rotate(240deg); }
    .p10 { transform: translate(-50%, 0) rotate(270deg); }
    .p11 { transform: translate(-50%, 0) rotate(300deg); }
    .p12 { transform: translate(-50%, 0) rotate(330deg); }

    .intro-text {
      font-size: 0.98rem;
      line-height: 1.5;
      color: #6d4c41;
      margin-bottom: 20px;
    }

    .btn-open {
      background: linear-gradient(135deg, #fbc02d 0%, #f57f17 100%);
      color: #fff;
      border: none;
      padding: 13px 26px;
      font-size: 1.05rem;
      font-weight: 600;
      border-radius: 30px;
      cursor: pointer;
      box-shadow: 0 6px 18px rgba(245, 127, 23, 0.4);
      transition: all 0.25s ease;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .btn-open:hover {
      transform: translateY(-2px) scale(1.03);
      box-shadow: 0 8px 22px rgba(245, 127, 23, 0.5);
    }

    .letter {
      display: none;
      margin-top: 22px;
      background: #fffde7;
      border: 1px dashed #fbc02d;
      border-radius: 18px;
      padding: 20px;
      animation: popLetter 0.5s ease-out forwards;
    }

    @keyframes popLetter {
      from { opacity: 0; transform: scale(0.9); }
      to   { opacity: 1; transform: scale(1); }
    }

    .letter-content {
      font-family: 'Caveat', cursive;
      font-size: 1.45rem;
      line-height: 1.5;
      color: #3e2723;
      white-space: pre-line;
      text-align: left;
    }

    .letter-signature {
      margin-top: 15px;
      font-weight: bold;
      text-align: right;
      color: #e65100;
    }

    .petal {
      position: fixed;
      top: -30px;
      font-size: 22px;
      user-select: none;
      pointer-events: none;
      z-index: 1;
      animation: fallDown linear forwards;
    }

    @keyframes fallDown {
      to { transform: translateY(105vh) rotate(360deg); }
    }
  </style>
</head>
<body>

  <div class="main-card">
    <div class="date-tag">21 de Septiembre 🌼</div>
    <h1>¡Feliz Día de las Flores Amarillas!</h1>

    <div class="sunflower-wrap">
      <div class="petals-ring">
        <div class="petal-leaf p1"></div>
        <div class="petal-leaf p2"></div>
        <div class="petal-leaf p3"></div>
        <div class="petal-leaf p4"></div>
        <div class="petal-leaf p5"></div>
        <div class="petal-leaf p6"></div>
        <div class="petal-leaf p7"></div>
        <div class="petal-leaf p8"></div>
        <div class="petal-leaf p9"></div>
        <div class="petal-leaf p10"></div>
        <div class="petal-leaf p11"></div>
        <div class="petal-leaf p12"></div>
      </div>
      <div class="center-flower"></div>
    </div>

    <p class="intro-text">
      Dicen que regalar flores amarillas hoy significa prometer amor sincero
      y traer luz para toda la vida. Tengo algo especial para ti...
    </p>

    <button id="toggleBtn" class="btn-open" onclick="openCard()">
      <span>Toca para abrir tu carta</span> ✨
    </button>

    <div id="secretLetter" class="letter">
      <div class="letter-content">
Hoy inicia la primavera y no podía dejar pasar este 21 de septiembre sin recordarte lo importante que eres para mí.

Estas flores nunca se marchitarán, al igual que todo el cariño y la felicidad que traes a mis días. Gracias por iluminar mi mundo con tu sonrisa.
      </div>
      <div class="letter-signature">— Con todo mi amor 💛</div>
    </div>
  </div>

  <script>
    function openCard() {
      const letter = document.getElementById('secretLetter');
      const btn = document.getElementById('toggleBtn');

      letter.style.display = 'block';
      btn.style.display = 'none';

      for (let i = 0; i < 28; i++) {
        setTimeout(spawnPetal, i * 80);
      }
    }

    function spawnPetal() {
      const items = ['🌻', '🌼', '💛', '✨', '🌸'];
      const petal = document.createElement('div');
      petal.classList.add('petal');
      petal.innerText = items[Math.floor(Math.random() * items.length)];
      petal.style.left = (Math.random() * 95) + 'vw';
      petal.style.animationDuration = (Math.random() * 3 + 3) + 's';
      petal.style.opacity = Math.random() * 0.7 + 0.3;
      petal.style.fontSize = (Math.random() * 12 + 18) + 'px';

      document.body.appendChild(petal);

      setTimeout(() => { petal.remove(); }, 6000);
    }

    setInterval(spawnPetal, 450);
  </script>
</body>
</html>
```

---

## 💡 Ideas para Personalizar Aún Más

- Cambiar la paleta de colores en `background` y `linear-gradient`.
- Añadir música de fondo con `<audio autoplay loop>`.
- Insertar una foto de la pareja dentro de la tarjeta.
- Añadir más emojis o mensajes secretos adicionales.
- Programar la fecha para que se muestre dinámicamente con JavaScript.

---

## 📌 Notas Finales

- La página funciona **100% offline** una vez cargada, excepto las fuentes de Google (si no hay internet, se usan las fuentes por defecto del sistema).
- Compatible con **Chrome, Safari, Firefox y Edge** en móvil y escritorio.
- No requiere servidor, base de datos ni frameworks.

---

## 📜 Créditos

Creado como detalle romántico para el **21 de septiembre**, Día de las Flores Amarillas y comienzo de la primavera. 🌻💛

> *"Dicen que regalar flores amarillas hoy significa prometer amor sincero y traer luz para toda la vida."*
