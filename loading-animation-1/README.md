# 🔄 CSS 3D Rotating "LOADING" Animation (HTML + CSS Only)

This project showcases a 3D **rotating text animation** for the word **LOADING**, built entirely using HTML and CSS. Each letter rotates in sequence, creating a wave-like loading effect — perfect for splash screens or preloaders.

🎯 No JavaScript needed — just HTML, CSS, and clever use of `transform` and `animation-delay`.

---

## 🚀 Features

- Pure HTML + CSS animation
- 3D `rotateZ` text effect
- Sequential delays for a wave animation
- Responsive and centered on screen
- Even-letter color alternation

---

## 🧾 Full Code (Single File)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Loading...</title>
    <style>
        * {
            margin: 0;
            padding: 0;
        }
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }
        span {
            display: inline-block;
            transform-origin: 0% 70%;
            transform-style: preserve-3d;
            color: #185793;
            font-size: 50px;
            animation: animate 2.5s infinite linear;
        }

        span:nth-child(1) { animation-delay: 0s; }
        span:nth-child(2) { animation-delay: 0.1s; }
        span:nth-child(3) { animation-delay: 0.2s; }
        span:nth-child(4) { animation-delay: 0.3s; }
        span:nth-child(5) { animation-delay: 0.4s; }
        span:nth-child(6) { animation-delay: 0.5s; }
        span:nth-child(7) { animation-delay: 0.6s; }

        span:nth-child(even) {
            color: #931715;
        }

        @keyframes animate {
            35% {
                transform: rotateZ(360deg);
            }
            100% {
                transform: rotateZ(360deg);
            }
        }
    </style>
</head>
<body>
    <span>L</span>
    <span>O</span>
    <span>A</span>
    <span>D</span>
    <span>I</span>
    <span>N</span>
    <span>G</span>
</body>
</html>
