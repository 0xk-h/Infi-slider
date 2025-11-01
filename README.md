# 🌌 Infinite Image & Text Slider

A smooth, fully responsive **infinite sliding animation** built using **Tailwind CSS**.  
 Supports both **text and image sliders** with customizable direction, speed, and dimensions — ideal for hero sections, banners, or showcases.

---

## ✨ Features

- 🔁 **Infinite looping** — continuous animation with seamless transitions
- 🧭 **Bidirectional** — supports both normal and reverse sliding
- 🎨 **Fully customizable** — height, width, speed, and count controlled via CSS variables
- 🖋️ **Text + Image modes** — easily switch between display types
- 🧱 **Built with Tailwind CSS 4** — no extra dependencies or JavaScript
- 💡 **Hover pause + grayscale filter** for elegant visual interaction

---

## 🛠️ Tech Stack

| Layer      | Tool                                                               |
| ---------- | ------------------------------------------------------------------ |
| Styling    | [Tailwind CSS 4](https://tailwindcss.com)                          |
| Build Tool | [@tailwindcss/cli](https://www.npmjs.com/package/@tailwindcss/cli) |
| Language   | HTML / CSS                                                         |

---

## 📁 Folder Structure

```
infi-slider/
  ├── public/
  │   ├── ape2.jpg
  │   ├── ape3.jpg
  │   └── ...
  ├── style.css        # Main CSS with animations and Tailwind layers
  ├── output.css       # Compiled output (auto-generated)
  ├── index.html       # Example slider demo
  └── package.json
```

---

## ⚙️ Usage

### 1️⃣ Install dependencies

`npm install`

### 2️⃣ Run Tailwind in watch mode

`npm run dev`

### 3️⃣ Open `index.html`

Open it directly in your browser to preview the slider.

---

## 🧩 Customization

| Variable           | Description                          | Example                    |
| ------------------ | ------------------------------------ | -------------------------- |
| `--width`          | Width of each item                   | `--width: 140px`           |
| `--height`         | Height of each item                  | `--height: 160px`          |
| `--quantity`       | Number of items in the list          | `--quantity: 10`           |
| `--pos`            | Position of each element in sequence | `--pos: 1`                 |
| `[reverse="true"]` | Attribute to reverse direction       | `<div reverse="true" ...>` |

### 🔄 Animation Speed

In `style.css`, adjust:
`animation: infislide 10s linear infinite;`
to:
`animation: infislide 15s linear infinite;`
for a slower scroll (or lower for faster).

---

## 🧠 Structure Example

### 🔹 Text Slider

```html
<div style="--height: 50px; --width: 140px" class="slider">
  <div style="--quantity: 7" class="list">
    <div class="item" style="--pos: 1">
      <h1 class="names">Roronoa Zoro</h1>
    </div>
    <!-- more items -->
  </div>
</div>
```

### 🔹 Image Slider

```html
<div style="--height: 160px; --width: 140px" class="slider">
  <div reverse="true" style="--quantity: 11" class="list">
    <div class="item" style="--pos: 1">
      <img src="./public/ape2.jpg" alt="Ape_2" />
    </div>
    <!-- more images -->
  </div>
</div>
```

---

## 🎨 Hover Effects

- Pauses animation on hover
- Grayscale applied to inactive elements
- Highlighted element scales slightly and regains color

---

## 👤 Author

**Kishore Kumar J**  
 🔗 [GitHub](https://github.com/0xk-h) • [LinkedIn](https://www.linkedin.com/in/kishore-kumar-547a79329/)

---

> _"Simplicity isn’t a limitation — it’s the aesthetic of mastery."_
