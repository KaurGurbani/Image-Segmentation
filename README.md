# 🌍 Satellite Image Segmentation Using HSV – Practice Project

This repository contains a Python-based project that performs **image segmentation on satellite imagery** to distinguish between **vegetation** and **concrete regions**, using **HSV color space** and **masking techniques**.

---

## 📌 Project Overview

This was a **practice project** completed as part of my self-learning journey in data science and computer vision. The objective was to take a raw satellite image and process it to separate:

- 🌿 **Vegetation areas**
- 🏗️ **Concrete/built-up areas**

The segmentation was performed based on **color features** by converting the image from **BGR → RGB → HSV** format and applying **HSV-based thresholding** followed by **masking**.

---

## 🛠️ Tech Stack

- Python
- OpenCV
- NumPy
- Matplotlib
- Visual Studio (used as IDE)

---

## 🧠 Key Concepts Used

- Color space conversion (BGR → RGB → HSV)
- HSV thresholding
- Image masking
- Satellite imagery processing
- Pixel-based segmentation

---

## 🔍 How It Works

1. Load the input satellite image using OpenCV (`cv2.imread`).
2. Convert the image from BGR to RGB.
3. Convert the RGB image to HSV color space.
4. Define HSV ranges for vegetation and concrete areas.
5. Apply `cv2.inRange()` to create binary masks.
6. Use `cv2.bitwise_and()` to apply the masks and extract segmented regions.
7. Visualize the results using Matplotlib.

---


## 🚀 Future Improvements

- Automate HSV range detection using clustering or K-means
- Add GUI for interactive HSV tuning
- Test on multiple satellite image types
- Classify more land types (water, soil, etc.)

---

## 📚 Learning Reflections

This project helped me:
- Understand the importance of color spaces in image processing
- Practice working with real-world visual datasets
- Gain hands-on experience with OpenCV and pixel-level operations

---

## 📎 License

This project is open for learning and experimentation. Feel free to fork and explore!

---



