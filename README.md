# 🌞🌙 AI Day/Night Image Classifier

An AI-based image classification project that identifies whether an image represents **DAY** or **NIGHT** by analyzing its brightness.

The project uses **Python, OpenCV, and Gradio** to process an uploaded image and provide a simple classification result.

---

## 🎯 Aim

The aim of this project is to demonstrate how Artificial Intelligence and Computer Vision can classify images into different categories.

The system analyzes the brightness of an image and determines whether it was taken during the day or at night.

---

## ❓ Problem Statement

Humans can easily identify whether an image was taken during the day or night, but computers cannot naturally understand visual information.

Smart cameras, security systems, and automated devices may need to understand lighting conditions automatically.

Manually checking a large number of images can be time-consuming. Therefore, an automated image classification system can be used to identify whether an image represents day or night.

---

## 💡 Problem Solution

The system analyzes the uploaded image and calculates its average brightness.

A predefined brightness threshold is used for classification:

- If brightness is greater than `100` → **DAY**
- If brightness is `100` or less → **NIGHT**

This allows the system to automatically classify the image without manual checking.

---

## ⚙️ How It Works

The project follows these steps:

```text
Upload Image
     ↓
Convert Image to Grayscale
     ↓
Calculate Average Brightness
     ↓
Compare Brightness with Threshold
     ↓
 ┌───────────────┐
 │ Brightness >100│
 └───────┬───────┘
         ↓
    ┌────┴────┐
    ↓         ↓
   DAY      NIGHT
