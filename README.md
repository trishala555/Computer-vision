# 🎨 Color Detection using Computer Vision

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green.svg)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 📌 Overview
This project is an **interactive color detection system** that allows users to click anywhere on an image and instantly identify the **color name along with its RGB values**.

Unlike complex AI-based systems, this project uses a **simple RGB comparison algorithm** with a predefined dataset, making it fast, efficient, and beginner-friendly.

---

## 🎯 Features
✨ Click on any pixel to detect color  
🎨 Displays **color name + RGB values**  
⚡ Real-time response  
🧠 No machine learning required  
🖱️ Interactive UI using OpenCV  

---

## 🖼️ Demo

### 📸 Screenshot
![Demo Screenshot](assets/screenshot.png)

### 🎥 GIF Demo
![Demo GIF](assets/demo.gif)

---

## 🛠️ Tech Stack
- Python  
- OpenCV  
- Pandas  
- NumPy  
- Jupyter Notebook / Google Colab  

---

## 📂 Project Structure

---

## 📊 Dataset
The dataset (`colors.csv`) contains:
- Color Name  
- Hex Value  
- RGB Values  

Example:

---

## ⚙️ Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/your-username/color-detection.git
cd color-detection
pip install opencv-python pandas numpy
jupyter notebook
Colour detection.ipynb
python color_detection.py
def get_closest_color(R, G, B):
    minimum = float('inf')
    cname = ""
    
    for i in range(len(csv)):
        d = abs(R - int(csv.loc[i,"R"])) + \
            abs(G - int(csv.loc[i,"G"])) + \
            abs(B - int(csv.loc[i,"B"]))
            
        if d < minimum:
            minimum = d
            cname = csv.loc[i,"color_name"]
    
    return cname
