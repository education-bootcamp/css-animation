# 🎨 CSS Gradient Text Animation (One File)

This project showcases a beautiful **animated gradient text effect** using **only one HTML file** — no external CSS or image files needed.

📺 **YouTube Demo:**  
👉 [Watch on YouTube Shorts](https://www.youtube.com/shorts/LAXBUzY3NGk?feature=share)

---

## 🚀 Features

- ✅ One-file solution (HTML + CSS combined)
- ✅ Pure HTML and CSS — no JavaScript
- ✅ Smooth infinite gradient animation
- ✅ Fully responsive using `vw` units

---

## 📄 One File Code

Copy and paste this into a file named `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Gradient Text Animation</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #000;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    h1 {
      text-transform: uppercase;
      font-size: 15vw;
      background: linear-gradient(90deg, #ff6ec4, #7873f5, #6ed3cf, #ff6ec4);
      background-size: 300%;
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      animation: move 6s linear infinite;
    }

    @keyframes move {
      0% {
        background-position: 0% 50%;
      }
      100% {
        background-position: 100% 50%;
      }
    }
  </style>
</head>
<body>
  <h1>Hi Team</h1>
</body>
</html>
