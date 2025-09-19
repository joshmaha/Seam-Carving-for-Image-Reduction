# Seam Carving for Content-Aware Image Resizing

This repository contains my implementation of **Seam Carving**, a content-aware image resizing technique introduced by Shai Avidan and Ariel Shamir. The project was completed as part of my **Computer Vision course**.

Seam carving allows images to be resized while better preserving important content compared to standard scaling. It works by finding and removing "seams" (low-energy paths of pixels) in an image.

---

## 🚀 Features

* Compute energy maps using image gradients.
* Find vertical and horizontal seams using dynamic programming.
* Remove seams iteratively to reduce width and height.
* Compare seam carving results with standard resizing (`cv2.resize`).
* Implemented a custom Gaussian filter for energy calculation (without library functions).
* Visualized results with Matplotlib (side-by-side comparisons).
* Tested on multiple images, including examples of both **good** and **bad** outcomes.

---

## 📂 Project Structure

```
├── notebooks/
│   └── Joshua_Maharaj_PS1.ipynb    # Main project notebook
├── images/
│   ├── input/                      # Input images
│   ├── output/                     # Results (reduced width/height, comparisons)
├── utils/
│   ├── helpers.py                  # Helper functions (load_rgb, show_images, save_rgb, etc.)
├── README.md                       # Project description
```

---

## 📸 Results

### Horizontal Seam Reduction

<img width="1378" height="472" alt="image" src="https://github.com/user-attachments/assets/ac321fd6-d246-46b1-8a05-3c1fefe88350" />

### Energy Gradient Magnitude and Cumulative Horizontal and Vertical Mapping

<img width="1678" height="455" alt="image" src="https://github.com/user-attachments/assets/23bc0d0c-0bcf-4426-85d5-b6e32875b4c5" />

### Original Energy Mapping vs Gaussian Filter Energy Mapping

<img width="733" height="294" alt="image" src="https://github.com/user-attachments/assets/f5bdf8f2-ec43-4d2a-87bb-bd8cee76c07b" />

### Test Beach Image using Seam Carving vs Standard Resizing

<img width="840" height="176" alt="image" src="https://github.com/user-attachments/assets/1f8c3909-c38f-4f75-bae8-fdca60cb6994" />

---

## 📖 Completed Sections

* **Q1**: Implemented energy function and seam visualization.
* **Q2**: Reduced width and height by removing vertical and horizontal seams.
* **Q3**: Combined seam carving operations to reduce both dimensions.
* **Q4**: Displayed seams on multiple iterations.
* **Q5**: Modified energy function (Gaussian filter).
* **Q6**: Tested on different images — showcased both perceptually pleasing and unrealistic outcomes.

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/joshmaha/seam-carving.git
cd seam-carving
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Requirements:

* Python 3.8+
* NumPy
* OpenCV
* Matplotlib

---

## ✨ Acknowledgments

* Avidan, S., & Shamir, A. (2007). *Seam Carving for Content-Aware Image Resizing*.
* Numpy, OpenCV, and Matplotlib libraries.
