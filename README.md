# Automatic License Plate Detection (ALPR) 🚗🔎

**Automatic-License-Plate-Detection** is a computer-vision pipeline that detects vehicle license plates and extracts text using YOLOv8 for detection and OCR for character recognition. The system was developed as part of a research project and achieved **~92%** detection/recognition accuracy on the test set.

---

## 🔍 Features
- Real-time license plate detection using YOLOv8
- Plate region extraction + OCR (character segmentation & recognition)
- Preprocessing (denoising, thresholding) for robust performance
- Sample inference script for images and video
- Instructions to run locally and reproduce results

---

## 📂 Repo structure (example)
Automatic-License-Plate-Detection/
├── assets/ # sample images & demo GIF
├── models/ # small model configs (weights stored externally)
├── src/
│ ├── detect.py
│ ├── ocr.py
│ └── utils.py
├── notebooks/ # EDA / experiments (optional)
├── requirements.txt
├── README.md
└── LICENSE

yaml
Copy code

---

## 🔧 Quickstart (local)
1. Clone:
```bash
git clone https://github.com/shreyasng693/Automatic-License-Plate-Detection.git
cd Automatic-License-Plate-Detection
Install:

bash
Copy code
pip install -r requirements.txt
Download model weights (example):

Place YOLOv8 weights in models/ (link or instructions here)

Run inference on an image:

bash
Copy code
python src/detect.py --input assets/car1.jpg --output output.jpg
 Results 
Test accuracy: ~92% (detection + OCR pipeline)

Include sample assets/output.jpg and a short demo GIF (assets/demo.gif) showing detection → OCR.

📄 Research
Published as: “Automatic License Plate Recognition system” — Akshaya Institute of Technology, Tumkur (Paper ID: 169, 2025).
