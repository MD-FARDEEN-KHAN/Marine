🌊 Marine Environmental Monitoring Via Attention Enhanced Yolov10 For Debris Detection

YOLO-MES is a lightweight deep learning–based underwater garbage detection framework designed for real-time marine debris monitoring in resource-constrained environments such as underwater robots, AUVs, and IoT-enabled marine systems.
The model is built upon YOLOv10n and enhanced with marine-environment-specific optimizations to improve detection accuracy, robustness, and efficiency in underwater conditions.

📌 Overview

Marine pollution is a major threat to aquatic ecosystems and the blue economy. Detecting underwater debris is challenging due to:

Light absorption and scattering

Low contrast and color distortion

Complex backgrounds (sand, rocks, flora)

Limited computational resources on underwater devices

YOLO-MES addresses these challenges by integrating lightweight architectural enhancements and marine-specific training strategies into a real-time detection pipeline.

🚀 Key Features

⚡ Lightweight YOLOv10n-based architecture

🌊 Optimized for underwater visual conditions

🤖 Suitable for AUVs, ROVs, and edge devices

🎯 Improved detection of marine debris classes

📉 Reduced parameters and computational cost

⏱️ Real-time inference capability

📊 Enhanced localization accuracy

🧠 Methodology

YOLO-MES introduces targeted improvements over baseline YOLOv10n for underwater garbage detection:

Marine-aware feature extraction

Efficient neck design for multi-scale debris detection

Optimized anchor-free detection strategy

Lightweight training configuration

Underwater dataset augmentation strategies

🗂️ Project Structure
YOLO-MES/
│
├── dataset/                # Underwater garbage dataset
│   ├── images/
│   ├── labels/
│
├── models/                 # YOLO-MES architecture configs
│
├── training/               # Training scripts
│
├── inference/              # Detection scripts
│
├── utils/                  # Preprocessing & helpers
│
├── results/                # Outputs & evaluation
│
└── README.md

📊 Dataset

The model is trained on an underwater garbage detection dataset containing annotated images of marine debris such as:

Plastic bottles

Bags

Fishing nets

Metal cans

Tires

Miscellaneous debris

Dataset preprocessing includes:

Color correction for underwater images

Contrast enhancement

Data augmentation (blur, turbidity, distortion)

Multi-scale training

⚙️ Installation
# Clone repository
use git clone and repository link to clone

# Create environment
conda create -n yolomes python=3.10 -y
conda activate yolomes

# Install dependencies
pip install -r requirements.txt

🏋️ Training
python training/train.py \
  --data dataset.yaml \
  --cfg models/yolo_mes.yaml \
  --epochs 100 \
  --img 640

🔎 Inference
python inference/detect.py \
  --weights runs/train/yolo_mes/weights/best.pt \
  --source test_images/

📈 Results

YOLO-MES achieves:

Higher detection accuracy in underwater scenes

Better small-object localization

Reduced model size

Real-time FPS on edge hardware

Example outputs include bounding-box detection of underwater debris in complex marine environments.

🌍 Applications

Autonomous underwater vehicles (AUVs)

Marine pollution monitoring systems

Smart ocean cleanup robots

Environmental research

Coastal surveillance

Underwater inspection

🔬 Research Contribution

This work proposes a lightweight marine-optimized YOLO detection scheme that balances:

Accuracy

Efficiency

Real-time performance

Edge deployability

It demonstrates that task-specific lightweight adaptation of modern YOLO architectures can significantly improve underwater debris detection.

👨‍💻 Author

MD Fardeen Ismail Khan
B.Tech CSE (AI & ML)
Lords Institute of Engineering and Technology

AI & Computer Vision Researcher

Underwater Object Detection

Edge AI Systems

GitHub: https://github.com/MD-FARDEEN-KHAN

LinkedIn: (add link)

📜 License

This project is released under the MIT License.

📢 Citation

If you use YOLO-MES in your research, please cite:

Fardeen, M. I. K. (2025).
YOLO-MES: An Effective Lightweight Underwater Garbage Detection Scheme
for Marine Ecosystems.

⭐ Acknowledgements

YOLOv10 authors

Underwater debris dataset contributors

Marine AI research community
