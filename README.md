---

#### **Project Overview**

This project aims to develop a robust fish detection model by leveraging transfer learning techniques and deploying the model on an embedded system (Raspberry Pi 4). The model is trained to accurately identify and segment various fish species in real-time, making it suitable for applications in marine biology, fishery management, and environmental monitoring.

The final goal is to prepare this project for research paper publication, demonstrating the practical applications and effectiveness of the developed model.

---

#### **Procedure**

1. **Dataset Preparation**
   - **CarMask Dataset**: Initially, a CarMask model was trained on a dataset designed to generate masks for cars.
   - **FishSpecies Dataset**: A dataset comprising various fish species was prepared for fine-tuning purposes.

2. **Model Fine-Tuning and Dataset Creation**
   - The CarMask model was fine-tuned using the FishSpecies dataset. This fine-tuning process enabled the model to generate accurate masks for different fish species, resulting in the creation of the **FishMask Dataset**.

3. **Transfer Learning and Model Training**
   - The FishMask dataset was integrated into Roboflow and further used to train a YOLOv8 model, producing the **FishMask Model**.
   - The FishMask Model was then further refined through additional YOLOv8 training using the FishSpecies dataset, resulting in the final **FishDetect Model**.

4. **Deployment**
   - The FishDetect Model was deployed on a Raspberry Pi 4, making it capable of real-time fish detection and segmentation.

---

#### **Accuracy Metrics**

- **Validation Results**: The model has shown exceptional performance across multiple fish species, with precision, recall, and mAP (mean Average Precision) metrics reflecting high accuracy:
   - **Overall mAP (50-95)**: 0.77
   - **Class-Specific Performance**:
     - **Gilt-Head Bream**: mAP - 0.791
     - **Red Sea Bream**: mAP - 0.79
     - **Striped Red Mullet**: mAP - 0.705
     - **Black Sea Sprat**: mAP - 0.767
     - **House Mackerel**: mAP - 0.804
     - **Red Mullet**: mAP - 0.766
     - **Sea Bass**: mAP - 0.804
     - **Shrimp**: mAP - 0.714
     - **Trout**: mAP - 0.789

These metrics highlight the model's effectiveness in accurately detecting and classifying various fish species.

---

#### **Future Work**

- **Optimization**: Ongoing efforts are focused on further optimizing the model's performance on the Raspberry Pi 4, ensuring it meets real-time processing requirements without sacrificing accuracy.
- **Field Testing**: The next phase will involve field testing in real-world aquatic environments to validate the model's robustness and adaptability.
- **Research Paper Publication**: Once the project reaches its final stages, the findings, methodology, and results will be documented and submitted for publication in a reputable research journal.

This project is currently under active development, and the upcoming phases will include further refinements and validations to prepare it for both practical deployment and academic contribution. The final research publication will include detailed technical insights, data analysis, and results, contributing valuable knowledge to the field of computer vision in marine applications.

---
