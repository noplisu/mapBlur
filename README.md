# 🗺️ Map Blur with Sharp Points of Interest (POIs)

This project demonstrates how to create a **Mapbox GL JS** map with a **blurred overlay**, while keeping specific **points of interest (POIs) sharp and visible**.

🌐 **Live Demo:** [noplisu.github.io/mapBlur](https://noplisu.github.io/mapBlur/)

---

## ✨ Features

- Uses **Mapbox GL JS v3.10.0**
- Adds a **blurred canvas layer** on top of the map
- Dynamically projects selected **POI coordinates into sharp circular zones**
- **Radius adjusts with zoom level** for better UX
- Handles **canvas resizing and re-rendering** on map movement

---

## 📍 Points of Interest (POIs)

The following cities in Poland are highlighted:

- Gliwice (`[18.6664, 50.2940]`)
- Kraków (`[19.9379, 50.0623]`)
- Warszawa (`[21.0031, 52.2290]`)

You can easily customize these in the `pois` array in the JavaScript section.

---

## 🧠 How It Works

1. A canvas is placed over the map container.
2. The map is drawn into this canvas.
3. Using the `ctx.clip()` method, circular regions corresponding to POIs are carved out.
4. The `filter: blur()` CSS property is applied to the canvas, blurring everything **except** those sharp circular areas.

---

## 🛠 Usage

You can clone this repo and host it via GitHub Pages or locally with any static file server.

```bash
git clone https://github.com/noplisu/mapBlur.git
cd mapBlur
open index.html
```

Or simply visit the hosted version at: 👉 [https://noplisu.github.io/mapBlur/](https://noplisu.github.io/mapBlur/)

---

## 🗝️ Mapbox Access Token

This project uses a public Mapbox access token. For public demos, this is acceptable. However, for production apps or private usage:

- Generate your own token from [Mapbox Account Dashboard](https://account.mapbox.com/)
- Restrict the token to specific domains or scopes as needed

---

## 📄 License

This project is licensed under the MIT License.

---

Made with ❤️ using [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/)

