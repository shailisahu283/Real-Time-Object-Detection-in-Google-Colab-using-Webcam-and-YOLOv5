# Real-Time Object Detection in Google Colab using Webcam and YOLOv5

This project demonstrates **real-time object detection** using your webcam directly inside **Google Colab**, with live bounding boxes drawn over detected objects using a YOLOv5 model.

---

## 📑 Table of Contents

* [📌 Features](#-features)
* [📁 Project Structure](#-project-structure)
* [✅ Requirements](#-requirements)
* [▶️ How to Run](#️-how-to-run)
* [🔍 How It Works](#-how-it-works)
* [🧠 Model Used](#-model-used)
* [⚙️ Tech Stack](#-tech-stack)
* [✨ Special Highlights](#-special-highlights)
* [🛑 Limitations](#-limitations)
* [📸 Example Output](#-example-output)
* [🙏 Acknowledgments](#-acknowledgments)

---

## 📌 Features

* 📷 Real-time webcam integration in Colab (via JavaScript).
* 🧠 Object detection using YOLOv5 (v5su variant).
* 🎯 Bounding box overlay on live video feed.
* 🧱 Uses OpenCV and PyTorch-based `ultralytics` library.
* 💡 Interactive—click video or instruction to stop detection.

---

## 📁 Project Structure

* `Object_Detection.ipynb` – Main Colab notebook containing all code.
* JavaScript functions embedded to handle webcam streaming inside the notebook.
* YOLOv5 lightweight model (`yolov5su.pt`) for object detection.

---

## ✅ Requirements

No local installation is required if using Google Colab.

Inside Colab, run:

```bash
!pip install opencv-python
!pip install ultralytics
```

---

## ▶️ How to Run

1. **Open the notebook** in Google Colab.
2. **Run all cells one by one** to:

   * Install dependencies
   * Start webcam streaming
   * Load YOLOv5 model
   * Run object detection
3. **Allow webcam permission** when prompted by the browser.
4. Detected objects will be highlighted live with bounding boxes.
5. **Click the video or red text to stop** the demo.

---

## 🔍 How It Works

* Webcam input is streamed using embedded **JavaScript**.
* Each frame is sent to Python as a base64-encoded image.
* YOLOv5 processes the frame and detects objects.
* Detected object bounding boxes are drawn as transparent overlays.
* These overlays are shown live on the next frame.

---

## 🧠 Model Used

* `yolov5su.pt`: A smaller, faster YOLOv5 variant from [Ultralytics](https://github.com/ultralytics/ultralytics).
* Optimized for fast inference in resource-constrained environments like Colab.

---

## ⚙️ Tech Stack

* Python
* JavaScript (for streaming UI)
* OpenCV
* Pillow (PIL)
* NumPy
* Ultralytics YOLOv5
* Google Colab

---

## ✨ Special Highlights

* 💻 Fully browser-based webcam streaming
* 🧠 Combines deep learning with interactive frontend
* 🛠️ Can be extended to custom object detection models

---

## 🛑 Limitations

* Frame delay due to Colab's processing (\~1 second latency).
* Not fully supported on all browsers (e.g., Safari may have issues).
* Click-to-stop might not always work on mobile browsers.

---

## 📸 Example Output



---

## 🙏 Acknowledgments

* Huge thanks to [Ultralytics](https://github.com/ultralytics/ultralytics) for their open-source YOLOv5 models.
* Inspired by the interactive webcam streaming tutorials by **Google Colab's Demos** and **fast.ai**.
* Built with ❤️ by **\Shaili Sahu**, as part of an educational and experimental deep learning project.
