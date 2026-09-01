🖼️ Minify Image – Electron Desktop App
=======================================

A lightweight **Electron desktop application** that compresses JPEG and PNG images with a single click. Pick an image, choose a quality level with a slider, and get a minified copy saved straight to your home directory.

Built with **Electron**, **imagemin**, **mozjpeg**, and **pngquant**, wrapped in a clean **Materialize CSS** UI.

* * *

🚀 Features
-----------

### 🗜️ Image Compression

*   Compresses **JPEG** images via `imagemin-mozjpeg`
*   Compresses **PNG** images via `imagemin-pngquant`
*   Single-file selection through a native file browser

### 🎚️ Quality Control

*   Adjustable quality slider (0–100)
*   Lower quality = smaller file size, higher quality = better fidelity

### 📁 Output Handling

*   Minified images are saved to `~/minifyimage`
*   Output folder opens automatically once compression finishes
*   Toast notification confirms completion with the quality used

### 🖥️ Native Desktop Experience

*   Cross-platform: **Windows**, **macOS**, and **Linux**
*   Native application menu with an **About** window
*   Dev tools and window resizing auto-enabled in development mode

* * *

🛠️ Tech Stack
--------------

*   **Framework:** Electron
*   **Image Processing:** imagemin, imagemin-mozjpeg, imagemin-pngquant
*   **Logging:** electron-log
*   **UI:** Materialize CSS, Font Awesome
*   **Path Handling:** slash
*   **Packaging:** electron-packager

* * *

📂 Project Structure
--------------------

```
image-minify/
├── app/
│   ├── index.html        # Main window UI
│   ├── about.html         # About window
│   ├── css/                # Materialize + custom styles
│   ├── js/                 # Materialize JS
│   └── webfonts/           # Font Awesome icon fonts
├── assets/
│   └── icons/               # App icons (Windows, macOS, Linux)
├── main.js                 # Electron main process
├── package.json
└── README.md
```

* * *

⚙️ Installation & Setup
-----------------------

### 1️⃣ Clone the repository
```bash
git clone https://github.com/mishraabhishek11/image-minify.git
```

### 2️⃣ Navigate to the project folder
```bash
cd image-minify
```

### 3️⃣ Install dependencies
```bash
npm install
```

### 4️⃣ Start the app
```bash
npm start
```

### 5️⃣ Run in development mode (auto-reload)
```bash
npm run dev
```

* * *

🧑‍💻 Usage
-----------

1.  Launch the app with `npm start`
2.  Click **Browse** and select a JPEG or PNG image
3.  Drag the **Quality** slider to your desired compression level
4.  Click **Resize** to compress the image
5.  The output folder (`~/minifyimage`) opens automatically with your minified image

* * *

📦 Building Distributables
---------------------------

Package the app into a standalone executable for your target platform:

```bash
# Windows
npm run package-win

# macOS
npm run package-mac

# Linux
npm run package-linux
```

Builds are output to the `release-builds/` directory.

* * *

🔮 Future Enhancements
----------------------

*   Batch/multi-image compression
*   Drag-and-drop image upload
*   Support for additional formats (WebP, AVIF)
*   Configurable output directory
*   Before/after file size comparison

* * *

🤝 Contributing
---------------

1.  Fork the repository
2.  Create a new branch (`git checkout -b feat/your-feature`)
3.  Make your changes
4.  Commit (`git commit -m "feat: add your feature"`)
5.  Push and open a Pull Request

* * *

📄 License
----------

This project is licensed under the **MIT License**.

* * *

👨‍💻 Author
------------

Abhishek Mishra

* * *

⭐ Support
---------

If you find this project useful, give it a ⭐ on GitHub!
