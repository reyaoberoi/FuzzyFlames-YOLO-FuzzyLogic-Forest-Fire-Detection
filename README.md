# Fuzzy Flames: A Hybrid YOLO–Fuzzy Logic Model for Early Detection of Forest Fires
This project implements a hybrid AI-based system for early forest fire detection and risk assessment using computer vision and fuzzy logic. The system combines YOLOv8 object detection with a fuzzy inference engine to not only detect fire regions in thermal imagery, but also classify fire severity levels in real time.

The model processes thermal images and video frames to identify fire hotspots, extracts features such as flame intensity, hotspot size, and detection confidence, and applies fuzzy logic rules to generate interpretable fire risk levels ranging from Low to Extreme. This approach significantly improves detection reliability while reducing false alarms compared to traditional threshold-based or YOLO-only methods. 

---

## Key Features

* Real-time forest fire detection using YOLOv8
* Fuzzy logic–based fire risk classification
* Interpretable severity levels (Low, Moderate, High, Very High, Extreme)
* Reduced false positives through contextual risk assessment
* Designed for UAV/drone and thermal imaging use cases

---

## System Architecture

1. Thermal images or video frames are captured (UAV or dataset input)
2. YOLOv8 detects fire regions and outputs bounding boxes with confidence scores
3. Flame intensity and hotspot size are computed from detected regions
4. A fuzzy inference system evaluates fire risk using expert-defined rules
5. Fire risk labels are visualized alongside detections in real time

---

## Technologies Used

* Python
* YOLOv8 (Ultralytics)
* OpenCV
* scikit-fuzzy
* NumPy, Matplotlib
* Google Colab / GPU environment
* Linux (Ubuntu)

---

## Dataset

* FLAME-3 Thermal Fire Dataset (fire and non-fire thermal imagery)
* Additional drone-based thermal video samples for evaluation

---

## Results

The hybrid YOLOv8 + fuzzy logic framework achieved higher accuracy and recall while significantly reducing false alarm rates compared to threshold-only and YOLO-only detection approaches. The fuzzy inference layer improves decision-making by incorporating contextual fire characteristics beyond raw model confidence. 

---

## Use Cases

* Early wildfire detection and monitoring
* UAV-based environmental surveillance
* Disaster management and emergency response systems
* Research and experimentation in explainable AI for safety-critical systems

---

## Future Improvements

* Integration of real-time environmental sensor data (wind, humidity, temperature)
* Expansion to adaptive neuro-fuzzy inference systems (ANFIS)
* Cloud-based deployment for real-time alerts and centralized monitoring
* Larger and more diverse training datasets
