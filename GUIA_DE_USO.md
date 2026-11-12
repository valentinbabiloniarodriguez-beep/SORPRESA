# 🎂 GUÍA DE USO Y PERSONALIZACIÓN: REGALO DE CUMPLEAÑOS PARA SARA

Esta experiencia web interactiva fue diseñada especialmente para **Sara** como un regalo digital elegante, emotivo y memorable, de parte de **Luis**.

---

## 🌐 Enlace Oficial en Vivo

Tu regalo ya se encuentra publicado y en línea de forma gratuita, segura y permanente en GitHub Pages:

👉 **[https://valentinbabiloniarodriguez-beep.github.io/SORPRESA/](https://valentinbabiloniarodriguez-beep.github.io/SORPRESA/)**

---

## 📖 Las 5 Escenas de la Experiencia

1. **Capítulo 1: Una sorpresa para Sara**
   - Fondo nocturno en tonos amatista y oro con partículas flotantes y luciérnagas.
   - Sobre interactivo 3D con sello decorativo de lacre.
   - Al pulsar *"Descubrir sorpresa ✨"*, la música (*Golden Hour*) comienza a sonar automáticamente, el sobre se abre y da paso a la celebración.

2. **Capítulo 2: ¡Feliz Cumpleaños!**
   - Torta de cumpleaños de dos pisos con glaseado y velas encendidas con animación de fuego titilante.
   - Lluvia de confeti celebratorio.
   - **Interacción especial:** Al tocar *"Pedir un deseo ✨"*, las velas se apagan con una suave estela de humo, suena una campana mágica y se revela el mensaje:  
     *«Que todos esos deseos que guardas en tu corazón encuentren el camino para hacerse realidad.»*

3. **Capítulo 3: Un Detalle que Florece**
   - Ramo floral bioluminiscente generado en código (curvas bézier orgánicas, hojas esmeralda y pétalos 3D en oro radiante, lavanda y rosa pastel).
   - Frase central de aprecio y cariño:  
     *«Porque las personas especiales merecen detalles que hagan florecer sus días.»*

4. **Capítulo 4: Recuerdos y una Carta para Ti**
   - **Galería Polaroid:** 3 tarjetas estilo scrapbook con cinta adhesiva superior y sombras suaves. Al tocarlas, se abre un visor (*lightbox*) para verlas en grande.
   - **Pestaña "Tu Carta ✉️":** Una carta en pergamino con las palabras dedicadas por Luis, redactadas con un tono sincero, cálido y de aprecio genuino.

5. **Capítulo 5: Gran Celebración Final**
   - Cierre festivo con estrellas doradas, confeti y aura celestial.
   - Mensaje de buenos deseos para este nuevo año de vida firmado por Luis.
   - Botón *"↺ Volver a vivir la sorpresa"* que reinicia toda la experiencia limpiamente.

---

## ⚙️ Cómo Personalizar el Contenido Fácilmente

Toda la configuración del proyecto se encuentra centralizada en las primeras líneas del archivo `<script id="birthday-engine">` dentro de [`index.html`](index.html).

### 1. Cambiar los nombres o mensajes:
Abre `index.html` con cualquier editor de texto (Bloc de Notas, VS Code, etc.) y busca el objeto `BIRTHDAY_CONFIG`:

```javascript
const BIRTHDAY_CONFIG = {
  recipient: "Sara",
  sender: "Luis",
  ...
};
```

### 2. Cómo agregar fotografías reales a la galería Polaroid:
Por defecto, las 3 tarjetas muestran una hermosa ilustración festiva para que la página luzca perfecta desde el primer momento. Si deseas agregar fotos reales de Sara o recuerdos:

1. Coloca tus archivos de imagen (por ejemplo `sara_foto1.jpg`, `sara_foto2.jpg`) en la misma carpeta `FLORES`.
2. En `index.html`, dentro de `BIRTHDAY_CONFIG.scene4.photos`, escribe el nombre del archivo en la propiedad `url`:

```javascript
photos: [
  {
    url: "sara_foto1.jpg", 
    caption: "Sonrisas y buenos momentos ✨",
    icon: "🎉"
  },
  {
    url: "sara_foto2.jpg", 
    caption: "Nuevos sueños por cumplir 🎯",
    icon: "🌟"
  },
  {
    url: "sara_foto3.jpg", 
    caption: "Un año extraordinario 💖",
    icon: "🎂"
  }
]
```

### 3. Cómo cambiar la música:
La música configurada es `Love1.mpeg`, ubicada en la misma carpeta del proyecto.
- Si deseas cambiarla por otra canción, simplemente coloca tu archivo de audio (por ejemplo `mi_cancion.mp3`) en la carpeta y actualiza:

```javascript
music: {
  url: "mi_cancion.mp3",
  volume: 0.85,
  loop: true
}
```

---

## 📲 Cómo Compartir el Enlace por WhatsApp

1. Abre la conversación con Sara en WhatsApp.
2. Pega el enlace:  
   `https://valentinbabiloniarodriguez-beep.github.io/SORPRESA/`
3. **Espera 2 a 3 segundos antes de presionar Enviar:** WhatsApp generará automáticamente la tarjeta de vista previa con el título *«¡Feliz Cumpleaños, Sara! 🎂✨»* y la descripción.
4. Puedes acompañarlo con este mensaje:

> *«Sara, hoy es un día especial... Preparé algo para ti. Ábrelo cuando tengas un momento tranquilo y activa el volumen 🎧✨»*  
> https://valentinbabiloniarodriguez-beep.github.io/SORPRESA/
