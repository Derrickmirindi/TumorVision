<img width="512" height="512" alt="1815" src="https://github.com/user-attachments/assets/b8b86d07-e01f-480c-a5ef-761297285a4a" />
# NeuroScan — Brain Tumor Detection

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://derrickmirindi.github.io/AI-Brain-Tumor/)
[![GitHub Pages](https://img.shields.io/badge/deployed-GitHub%20Pages-blue)](https://derrickmirindi.github.io/AI-Brain-Tumor/)
[![ONNX](https://img.shields.io/badge/model-ONNX-orange)](https://onnx.ai/)

Real-time brain tumor detection using YOLO11s segmentation, running entirely in your browser via ONNX Runtime Web.

## 🚀 Live Demo

**Try it now:** [https://derrickmirindi.github.io/AI-Brain-Tumor/](https://derrickmirindi.github.io/AI-Brain-Tumor/)

## ✨ Features

- **Client-Side Inference** — All processing happens locally in your browser; no server uploads, complete privacy
- **Fast Loading** — 19MB model cached locally after first load (loads instantly on repeat visits)
- **Progress Tracking** — Real-time download progress bar for first-time visitors
- **Multiple Input Modes** — Upload images, videos, or use live webcam
- **Adjustable Parameters** — Confidence threshold and IoU sliders for fine-tuning
- **Real-Time Detection** — Live camera mode for instant tumor detection
- **Responsive UI** — Works on desktop and mobile browsers

## 🧠 How It Works

1. **Upload** an MRI scan image (or use video/webcam mode)
2. **Inference** runs locally using ONNX Runtime WebAssembly
3. **Results** display bounding boxes with confidence scores
4. **Export** detection stats (count, max confidence, inference time)

### Technical Stack

- **Model**: YOLO11s segmentation trained on brain tumor MRI dataset
- **Format**: ONNX (Open Neural Network Exchange)
- **Runtime**: ONNX Runtime Web (WebAssembly)
- **Frontend**: Vanilla HTML/CSS/JavaScript (no frameworks)
- **Deployment**: GitHub Pages (static hosting)

## 📊 Performance

- **Model Size**: 19.4 MB (ONNX format)
- **Inference Speed**: ~900ms per image (browser-dependent)
- **Input Size**: 640x640 pixels
- **Output**: Bounding boxes with class probabilities

## 🔧 Local Development

```bash
# Clone the repository
git clone https://github.com/Derrickmirindi/AI-Brain-Tumor.git
cd AI-Brain-Tumor

# Serve locally (any static server)
python -m http.server 8000
# or
npx serve

# Open http://localhost:8000
```

## 📁 Repository Structure

```
.
├── index.html      # Single-page app with embedded CSS/JS
├── best.onnx       # YOLO11s tumor detection model
└── README.md       # This file
```

## ⚠️ Disclaimer

**FOR RESEARCH AND EDUCATIONAL USE ONLY**

This application is NOT a medical device and must NEVER be used for clinical diagnosis or treatment decisions. Always consult qualified healthcare professionals for medical advice.

## 📄 License

MIT License - feel free to use this project for research and education.

## 🤝 Contributing

Contributions welcome! Open an issue or submit a pull request.

## 📧 Contact

Developed by [Derrick Mirindi](https://github.com/Derrickmirindi)

---

**Note**: First load downloads the 19MB model with a progress bar. Subsequent visits load instantly from browser cache.
