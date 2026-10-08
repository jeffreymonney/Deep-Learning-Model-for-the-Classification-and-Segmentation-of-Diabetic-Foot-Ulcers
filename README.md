# Deep-Learning-Model-for-the-Classification-and-Segmentation-of-Diabetic-Foot-Ulcers
This project develops an AI-powered system for early diabetic foot ulcer detection, wound segmentation, severity classification, and explainable assessment, with progression tracking and mobile application integration for accessible healthcare support.
## Project Description

DFUDetect is an enhanced deep learning system developed to support the early detection, segmentation, and severity assessment of Diabetic Foot Ulcers (DFUs). The project combines computer vision, deep learning, explainable AI, and mobile application technologies to provide an accessible approach to DFU assessment.

The system uses a **two-stage deep learning pipeline**. First, **ResUNet** is used to perform pixel-level wound segmentation and identify the ulcer region from a foot image. The segmented region is then extracted as a **Region of Interest (ROI)** and passed to **EfficientNet-B3**, which classifies the wound into the defined severity categories. **Grad-CAM** is also integrated to provide visual heatmaps showing the areas that influenced the classification result.

The project was developed using **Python and TensorFlow/Keras**, with **OpenCV, NumPy, Pandas, and Scikit-learn** supporting image processing, data preparation, and model evaluation. **Google Colab** was used for model development and training, while **Google Drive** was used for dataset and model storage.

For deployment, a **Flask REST API** was developed as the backend to connect the trained models with the application. The backend manages image uploads, preprocessing, segmentation, ROI extraction, classification, Grad-CAM generation, and prediction results. A progression component was also developed to support monitoring of wound-area and severity changes across multiple assessments.

A **Flutter and Dart** mobile application provides the user interface, allowing users to capture or upload foot images and view the analysis results. The overall system is designed to provide an explainable and accessible AI-assisted solution, particularly for healthcare environments with limited resources.

The project demonstrates how deep learning and mobile technologies can be combined to support earlier and more consistent diabetic foot ulcer assessment, while recognizing that clinical validation is required before real-world medical deployment.
