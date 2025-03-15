# ML-Based Image Classification of Mineral Ore using YOLOv9 🚀

## Introduction 🌐
The **ML-Based Image Classification of Mineral Ore** project utilizes the advanced **YOLOv9 (You Only Look Once version 9)** algorithm to accurately classify mineral ores into distinct categories based on their size and characteristics. This project addresses the challenges of manual ore classification, which is prone to human error and inefficiencies, by implementing a robust and automated solution.

### Motivation 💡
Traditional mineral classification methods in mining are labor-intensive and error-prone. This project aims to enhance operational efficiency by leveraging **YOLOv9** for real-time, automated classification of mineral ores. The model efficiently distinguishes between **lumps** and **fines**, significantly reducing manual effort and improving accuracy.

---

## Features 🚀
- **Real-Time Classification:** Quickly identifies and categorizes mineral ore.
- **High Accuracy:** Uses YOLOv9's object detection capabilities for precise results.
- **Data Augmentation:** Incorporates various transformations to improve robustness.
- **Advanced Architecture:** Employs **GELAN (Generalized Efficient Layer Aggregation Network)** and **PGI (Programmable Gradient Information)**.
- **Custom Models:** Supports both **Single** and **Multiple Annotation** models.
- **Web App Integration:** Provides an interactive interface for real-time predictions.

---

## Project Structure 📂
```
├── data/                   # Datasets and pre-trained models
├── scripts/                # Python scripts for training and inference
├── models/                 # YOLOv9 model configurations
├── utils/                  # Utility functions and tools
├── results/                # Outputs and performance metrics
├── docs/                   # Documentation and reports
├── experiments/            # Experimental models and tests
├── README.md               # Project documentation
└── requirements.txt        # List of dependencies
```

---

## Installation 🛠️

### Prerequisites
- Python 3.8+
- PyTorch 1.7+
- CUDA (for GPU support)
- Git
- pip

### Clone the Repository
```
git clone https://github.com/username/mineral-ore-classification-yolov9.git
cd mineral-ore-classification-yolov9
```

### Install Dependencies
```
pip install -r requirements.txt
```

### Download Pre-trained Weights
```
wget https://github.com/WongKinYiu/yolov9/releases/download/v0.1/yolov9-c.pt
```

---

## Usage 💻

### Training the Model 🏋️‍♂️
To train the model on a custom dataset:
```
python scripts/train.py --data data/ore.yaml --cfg models/yolov9.yaml --epochs 50
```

### Real-Time Inference 📸
#### Using a Webcam
```
python scripts/detect.py --source 0 --weights models/yolov9-c.pt
```

#### Using a Video File
```
python scripts/detect.py --source path/to/video.mp4 --weights models/yolov9-c.pt
```

#### Viewing Results
Outputs are saved in the `results/` directory with labeled bounding boxes and classifications.

---

## Results and Performance 📊
| Metric                   | Single Annotation | Multiple Annotation |
|--------------------------|-------------------|----------------------|
| mAP (Mean Average Precision) | 99.5%             | 11.6%                |
| Precision                | 98.6%             | 21.1%                |
| Recall                   | 100.0%            | 13.7%                |

### Visualization
- **Confusion Matrix:** Evaluates detection accuracy and false positives.
- **Precision-Recall Curve:** Analyzes the balance between precision and recall.
- **Loss Curves:** Tracks model optimization and convergence.

---

## Limitations 🚧
- **Dataset Dependency:** Requires a diverse and well-annotated dataset.
- **Computationally Intensive:** High-performance GPU required for real-time applications.
- **Environmental Sensitivity:** Performance varies with lighting and noise.

---

## Future Enhancements 🌱
- **Lightweight Models:** Optimize for low-power devices.
- **Real-Time Deployment:** Integrate with IoT devices for field applications.
- **Advanced Augmentation:** Improve robustness under varying conditions.

---

## Contributing 🤝
Contributions are welcome! Please fork the repository, create a new branch, and submit a pull request.

### Guidelines
- Follow PEP8 for code formatting.
- Include tests and documentation for new features.

---

## License 📄
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---

## Acknowledgements 🙏
- **CSM Technologies** for guidance and support.
- **Sikkim Manipal Institute of Technology** for infrastructure and mentorship.
- **Roboflow** for dataset management and augmentation tools.

---

## Authors ✍️
- **Ricky Mohanty** (Reg. No. 202000358)
- Guided by **Mr. Sanjay Kumar**, Data Scientist, CSM Technologies


