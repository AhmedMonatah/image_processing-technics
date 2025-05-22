# 🖼️ Image Processing & ORB Feature Detection with OpenCV

A Colab-based image processing pipeline that allows you to upload an image, enhance it, apply filtering, and extract ORB features — all with visual feedback at each step.

---

## 📁 Project Overview

This project offers an end-to-end demonstration of fundamental image processing techniques using **OpenCV** and **NumPy** in a Python (Google Colab) environment. It performs:

- ✅ Brightness & Contrast Adjustment  
- ✅ Gaussian Blurring  
- ✅ Non-local Means Denoising  
- ✅ Canny Edge Detection  
- ✅ ORB Keypoint Detection  

All transformations are visualized using **Matplotlib**, making this project ideal for educational purposes, prototyping, or image preprocessing.

---

## ▶️ How to Run

> 🧠 This notebook is designed for **Google Colab**.

1. **Clone or copy the code into a Colab notebook.**
2. **Run the notebook cells sequentially.**
3. When prompted:
   - Upload an image (`.jpg`, `.jpeg`, `.png`, `.tif`, `.tiff`)
4. Observe the outputs:
   - Intermediate results will be displayed after each processing step.
5. (Optional) The project zips and downloads results at the end — make sure any saving code is configured properly.

---
## Techniques Used
- **Brightness/Contrast Adjustment**: Modifies pixel intensities to enhance image appearance.
- **Gaussian Blur**: Applies a 5x5 kernel to smooth the image and reduce detail.
- **Non-local Means Denoising**: Reduces noise while preserving edges using OpenCV's fastNlMeansDenoisingColored.
- **Canny Edge Detection**: Detects object boundaries using low (100) and high (200) thresholds.
- **ORB Feature Extraction**: Detects keypoints and computes descriptors for object characterization.

### Execution Steps:
1. Copy the complete script into a notebook cell.
2. Ensure the dataset is mounted at:

---

## 🔍 Known Limitations & Notes

- ⚠️ **Single Image Input**: The script currently supports uploading and processing one image at a time. Batch processing is not implemented.
- 💾 **Processed Image Not Saved by Default**: The processed images are only displayed. If you want to save them to disk, you must add explicit `cv2.imwrite()` statements.
- 🧠 **Colab Environment Limitation**: This code is tailored for Google Colab. Running it locally requires modifications for file handling (i.e., removing `files.upload()` and `files.download()`).
- 🎯 **ORB Sensitivity**: ORB feature detection may yield limited keypoints on low-texture or overly smooth images.
- 📦 **Download ZIP Requires Manual Saving**: The ZIP download at the end depends on manually saving images to a `processed_images/` directory first.
- 🧪 **No Error Feedback for Processing Steps**: While the upload has basic error handling, if one of the processing steps fails (e.g., a malformed image), it may not provide detailed feedback.
- 🌐 **No GUI Interface**: All interactions are handled via Colab's notebook cell prompts and visual outputs, without a graphical interface or buttons.

---
