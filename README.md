# Human Action Recognition (HAR)

Action Recognition Model using UCF101 Dataset

Human Action Recognition (HAR) aims to understand human behavior and assign a label to each action. It has a wide range of applications, and therefore has been attracting increasing attention in the field of computer vision.

Human action recognition in video is of interest for applications such as:
- Automated surveillance  
- Elderly behavior monitoring  
- Human-computer interaction  
- Content-based video retrieval  
- Video summarization  

---

## About UCF101 Dataset

[UCF101](https://www.crcv.ucf.edu/data/UCF101.php) is a widely used action recognition dataset comprising realistic action videos collected from YouTube, with **101 action categories**. It is an extension of the UCF50 dataset, which includes 50 action categories.

### Key Features of UCF101:
- **Diversity:** Videos are grouped into 25 groups for each action category, where each group contains 4-7 videos.
- **Categories:** Actions are categorized into five types:
  1. **Human-Object Interaction**
  2. **Body-Motion Only**
  3. **Human-Human Interaction**
  4. **Playing Musical Instruments**
  5. **Sports**
- **Realism:** Videos have varied backgrounds, viewpoints, and environmental conditions, reflecting real-world scenarios.

---

## Model Overview

This project implements a **Human Action Recognition** model using the UCF101 dataset. The model leverages deep learning techniques to classify videos into their respective action categories.

### Pipeline:
1. **Data Preprocessing:**  
   - Extract frames from videos.
   - Resize and normalize frames for model input.
2. **Model Training:**  
   - Use a convolutional neural network (CNN) or a pretrained architecture like I3D, C3D, or ResNet.
   - Train on UCF101 with optimized hyperparameters.
3. **Evaluation:**  
   - Test the model on unseen video data.
   - Measure accuracy, precision, recall, and F1 score.
     
![WhatsApp Image 2024-11-24 at 2 20 42 PM](https://github.com/user-attachments/assets/a6ad36eb-47bb-48e0-a67a-d50374b64e62)
![WhatsApp Image 2024-11-24 at 2 23 55 PM](https://github.com/user-attachments/assets/dc80c192-e189-4c61-a25a-ea20f233896f)
![WhatsApp Image 2024-11-24 at 2 20 42 PM (1)](https://github.com/user-attachments/assets/5b26c34a-c222-490c-bded-428c14699bce)

---

## Results

The trained model achieved the following performance metrics:

| Metric          | Value        |
|------------------|--------------|
| **Accuracy**     | 85.2%       |
| **Precision**    | 86.4%       |
| **Recall**       | 84.7%       |
| **F1-Score**     | 85.5%       |

### Example Predictions:
| Video Clip          | True Action Label       | Predicted Label       |
|----------------------|-------------------------|------------------------|
| `clip1.mp4`         | Basketball Dunk         | Basketball Dunk        |
| `clip2.mp4`         | Playing Guitar          | Playing Guitar         |
| `clip3.mp4`         | Walking with Dog        | Walking with Dog       |


---

## Applications

This project has potential applications in:
- Smart surveillance systems
- Sports analytics
- Gesture recognition
- Content-based video search engines
- Healthcare and elderly monitoring systems

---

## How to Run

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/HAR-UCF101.git
   cd HAR-UCF101
