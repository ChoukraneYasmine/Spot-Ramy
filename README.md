# Spot-Ramy
## 🏆 Algiers UP 2025 - 2nd Place Winner
Spot Ramy is an AI-powered mobile application designed for automatic product detection, classification, and counting in store shelves. This solution was developed during the AUP Hackathon, where the theme focused on merchandising and how to facilitate the work of merchandisers. Our team, SIQLID, proudly secured second place in this competition..

## Content
This repository contains the AI component of our solution, including:
- **Data Preprocessing**: Dataset annotation and data augmentation.
- **Object Detection**: Using YOLOv8 to detect products.
- **Classification**: Using ResNet18 to classify detected products.
- **Product Counting**: Analyzing and quantifying the detected products.

---

##  1. Data Preprocessing
The dataset of Ramy product images was provided by Ramy during the competition. It contains various labeled product images used for training and evaluation of our AI models.
 
To enhance our dataset, we also scraped images of competing products (e.g., Rouiba) using web scraping techniques.

### Key Steps:
- **Dataset Collection**: Annotated images of Ramy products.
- **Web Scraping**: Automated collection of competitor images.
- **Preprocessing**: Data cleaning and augmentation to improve model performance.

---

##  2. Object Detection with YOLOv8
We implemented YOLOv8 for object detection to identify bottled and canned products in store shelf images.

### Implementation:
- Used a pre-trained **YOLOv8 model** to detect objects.
- Filtered detections to focus on relevant product classes (bottles and cans).
- Cropped detected objects for further classification.


##  3. Product Classification with ResNet18
Once the products were detected, we classified them using a fine-tuned **ResNet18 model**.

### Training Process:
- Trained on labeled product images (Ramy and Rouiba).
- Used **PyTorch** and **transfer learning**.
- Evaluated using accuracy, precision, recall, and F1-score.


##  4. Product Counting
Using YOLO and ResNet predictions, we developed a **counting algorithm** to quantify each detected product type.

### Steps:
1. Detect and classify each product.
2. Store counts in a structured format.
3. Generate insights on stock availability.

## Team Members
- Herkat Wifak – Designer

- Khadir Amina – Mobile Developer

- Djedjig Nada – AI Developer

- Choukrane Yasmine – AI Developer




