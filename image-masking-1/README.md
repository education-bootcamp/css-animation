# 🌿 Transparent Paint Splash Overlay Effect (HTML + CSS)

This project shows how to use **a transparent paint splash PNG** layered over a fullscreen background using only HTML and CSS. The effect is achieved using a `::before` pseudo-element and `mix-blend-mode: screen`.

🎬 **Live Demo:**  
👉 https://youtube.com/shorts/rXzhvwKAR2U

---

## 🚀 Features

- Pure HTML + CSS (no JS)
- Fullscreen responsive layout
- `mix-blend-mode` for a blended overlay effect
- Transparent splash PNG layered with `::before`
- Works on all modern browsers

---

## 🧾 One-File Full Code (HTML + CSS Inline)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Paint Splash Overlay</title>
  <style>
    * {
      margin: 0;
    }

    body, html {
      height: 100%;
      width: 100%;
    }

    section {
      width: 100vw;
      height: 100vh;
      background: url("leaf-bg.jpg") center center no-repeat;
      background-size: cover;
      position: relative;
      overflow: hidden;
    }

    section::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url("transparent-paint-splash.png") center center no-repeat;
      background-size: cover;
      mix-blend-mode: screen;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <section></section>
</body>
</html>
