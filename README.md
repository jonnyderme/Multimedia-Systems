# 📸 Multimedia-Systems
Assignment for the "Multimedia Systems" Course  
Faculty of Engineering, AUTh  
School of Electrical and Computer Engineering  
Electronics and Computers Department

📚 *Course:* Multimedia Systems  
🏛️ *Faculty:* AUTh - School of Electrical and Computer Engineering  
📅 *Semester:* 9th Semester, 2023-24

---

## 📚 Table of Contents
- [Overview](#overview)
- [Part A: JPEG Library – Core Functions](#part-a-jpeg-library--core-functions)
- [Part B: JPEG Encoder / Decoder Integration](#part-b-jpeg-encoder--decoder-integration)
- [Part C: JPEG File Format & Stream](#part-c-jpeg-file-format--stream)
- [Repository Structure](#repository-structure)

---

## 🧠 Overview

This assignment involves building a simplified JPEG codec from scratch in Python, following the baseline sequential DCT-based JPEG standard. The project is divided into 3 parts, progressively integrating preprocessing, compression, and stream generation. Deliverables include documented `.py` files and a `report.pdf`.

---

## 🧩 Part A: JPEG Library – Core Functions

Implemented low-level modules for:
- RGB to YCrCb conversion with 4:4:4 / 4:2:2 / 4:2:0 subsampling
- DCT and inverse DCT using block-wise transforms
- Quantization and dequantization based on standard tables and scale
- Zig-zag scanning & run-length encoding
- Huffman coding using fixed standard tables
- 📄 Demo: `demo1.py` demonstrates encoding and reconstruction using 2 test images

---

## 🛠️ Part B: JPEG Encoder / Decoder Integration

- Encapsulates Part A into a high-level JPEG encoder/decoder
- Supports variable quantization scales and subsampling
- Produces compression metrics (MSE, bitrate, visual comparison)
- 📄 Demo: `demo2.py` calculates entropy in various domains and evaluates compression performance

---

## 🧾 Part C: JPEG File Format & Stream

- Generates a valid JPEG bitstream using standardized markers and format
- Final output is viewable in any standard image viewer
- Implements:
  - `JPEGencodeStream(img, subimg, qScale)`
  - `JPEGdecodeStream(encodedStream)`

---

## 📁 Repository Structure
```
├── Assignment/
│   └── itu-t81.pdf                            # JPEG specification reference document
│   └── auth_multimedia_2023_2024_hw1.pdf      # Assignment
├── Code/
│   └── Multimedia_Project_Deirmentzoglou_Ioannis_10015.py   # Python implementation of the JPEG pipeline
├── Images/
│   └── lena_color_512.png                     # Input test image used for compression
│   └── baboon_512.png                     # Input test image used for compression
├── Auth_Multimedia_Systems_Project.ipynb      # Main Colab notebook
└── README.md                                   # This documentation
```
