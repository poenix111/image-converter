# 📸 _Converter

A high-performance, client-side batch image converter built with **Astro** and styled using **Material Design 3 (M3)** guidelines. It allows you to process bulk image conversions (including modern Apple HEIC/HEIF files) directly in your browser with zero server latency, complete privacy, and full color gamut preservation.

---

## ✨ Features

- **🔒 100% Client-Side:** All decoding, conversion, and compression happen directly in the browser. Your photos never leave your device.
- **🚪 No Login Wall:** Instant access with no sign-ups, accounts, subscription limits, or log-in popups.
- **🍏 HEIC & HEIF Support:** Converts modern high-efficiency formats from Apple cameras on-the-fly to standard formats.
---

## 🛠️ Technology Stack

- **Framework:** [Astro](https://astro.build/) (Static Site Generation)
- **ZIP Compression:** [JSZip](https://stuk.github.io/jszip/) (Pure JS browser packaging)
- **HEIC Decoder:** [heic-to](https://github.com/alexcorvi/heic-to) (Dynamic import for WASM/Canvas decoding)
- **Graphics Pipeline:** HTML5 Canvas 2D API (Display-P3 color space configuration)

---

## 🚀 Getting Started

### 1. Install Dependencies
Run the following command from the root directory to download necessary node modules:
```bash
npm install
```

### 2. Run the Development Server
Launch the local Astro development server:
```bash
npm run dev
```
The application will be running at **[http://localhost:4321](http://localhost:4321)**.

### 3. Build for Production
To compile an optimized static build:
```bash
npm run build
```
The output static assets will be located in the `./dist/` directory.

### 4. Preview Production Build
Preview the production build locally before deployment:
```bash
npm run preview
```

---

## 📂 Project Structure

```text
/
├── public/
│   └── favicon.svg           # Favicon asset
├── src/
│   ├── components/
│   │   └── Converter.astro   # Main two-column converter dashboard, logic, and global styles
│   ├── layouts/
│   │   └── Layout.astro      # Global layout wrapper setting up Outfit typography and Material 3 variables
│   └── pages/
│       └── index.astro       # Landing entry page importing the Converter
├── package.json
└── README.md
```

---

## 👤 Author

Developed with ♥ by [poenix111](https://github.com/poenix111).
