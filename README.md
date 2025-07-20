# 🌍 Vegetation & Concrete Segmentation from Satellite Imagery (HSV-Based)

This repository showcases a **color-based image segmentation project** that identifies **vegetation** and **concrete/built-up areas** from satellite imagery using the **HSV color space** in **Python**.

---

## 📌 Project Description

As part of my self-learning in computer vision and geospatial data analysis, I developed this practice project to explore how color information in satellite images can be used to classify land surfaces. The image is segmented into:

- 🌿 **Vegetation zones**
- 🏗️ **Concrete/Bare ground areas**

The technique relies on transforming color space from **BGR → RGB → HSV**, then applying HSV-based thresholding and masking to isolate regions of interest.

---

## 🧪 Segmentation Pipeline

1. **Image Preprocessing**  
   - Load satellite image  
   - Convert from BGR → RGB → HSV  
   - Resize to 512x512 for consistent results

2. **HSV Channel Visualization**  
   - Analyze Hue, Saturation, and Value separately to define effective thresholds

3. **Color Thresholding**  
   - **Vegetation**: Hue 35–90, moderate Saturation & Value  
   - **Concrete**: Low Saturation (0–70), high Value (70–255), all Hue values

4. **Overlap Handling**  
   - Ensures no confusion between vegetation and concrete classification

5. **Mask Cleaning**  
   - Applies **morphological closing** (dilation + erosion) to reduce noise and improve segmentation quality

6. **Final Visualization**  
   - Output image shows:
     - Vegetation in dark green  
     - Concrete in gray  
     - Unclassified areas in black

---

## 🛠️ Tools & Libraries

- Python  
- OpenCV  
- NumPy  
- Matplotlib  
- Visual Studio (as IDE)

---

## 🖼️ Segmentation Outputs

Visual results from various stages of the segmentation pipeline:

### 🔹 Original Image (BGR)
<img src="images/BGR image.png" alt="BGR Image" width="400"/>

### 🔹 Converted to RGB
<img src="images/RGB image.png" alt="RGB Image" width="400"/>

### 🔹 HSV Channel Visualization
<img src="images/Hue channels.png" alt="Hue Channels" width="400"/>

### 🟢 Vegetation Area Segmentation
<img src="images/Vegetation area.png" alt="Vegetation Area" width="400"/>

### ⚪ Concrete Area Segmentation
<img src="images/Concrete area.png" alt="Concrete Area" width="400"/>

---

> 🎨 **Color Legend**  
> • Vegetation → 🟢 Dark Green  
> • Concrete/Built-Up → ⚪ Gray  
> • Unclassified → ⚫ Black

---

## 📚 What I Learned

- Image preprocessing and transformation techniques  
- Color space concepts and HSV thresholding  
- Morphological operations for mask refinement  
- Real-world relevance of segmentation in environmental and urban analysis

---

## 📄 License

This project is released under the MIT License. See the [LICENSE](./LICENSE) file for details.

---
