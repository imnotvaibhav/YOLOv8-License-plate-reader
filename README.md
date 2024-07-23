
# License Plate Detector

The project aims to develop an License Plate detection system for identifying and reading text from plates of vcarious vehicles in road traffic. Image dataset of Belgian car license plates is used. The project involves data preprocessing, training a YOLOv8 model, and deploying the model in a web application for practical use.

# 1. Dataset Overview
This is an image dataset of Belgian car license plates. This dataset already comes with well-annotated XML files. The dataset contains more than 433 images and 433 annotation files.

# 2. Data Pre-processing
The data pre-processing pipeline involves two main steps: identifying labels and formatting for the YOLOv8 algorithm. XML files are processed to extract labels enclosed in <object><name> tags. These labels are then mapped to numerical indices and stored in a dictionary. The data extraction process includes reading XML files, splitting content, and organizing labels into a unique set. Additionally, the YOLOv8 format requires extracting coordinates and dimensions, normalizing them, and writing the data to a text file. This process ensures that the data is appropriately formatted for training the YOLO model.

# 3. Model Training
The YOLOv8 model is trained using Ultralytics' object detection setup. The dataset is divided into training and testing sets, and the model is trained over 100 epochs. The training process involves optimizing the model's parameters to accurately detect and classify vehicles in the provided images. Model performance evaluation is conducted using the testing set to ensure its generalization capability.

# 4. Model Deployment
The trained YOLO model is deployed in a web application developed using streamlit. The web app allows users to upload images and videos of vehicles in .jpg, .jpeg, .png, .mp4, .mkv format. After clicking the upload button, the model performs object detection on the uploaded image and displays the image with detected vehicles' license plate highlighted and a probability score of prediction. The user-friendly interface enhances the accessibility and practicality of the developed object detection system.

# 5. Conclusion
The project successfully addresses the challenge of fine license plate reading in road traffic. The combination of meticulous data labeling, YOLOv8 model training, and web application deployment showcases a comprehensive approach to solving real-world problems of security and safety. The project's outcomes hold significant potential for practical applications, ranging from Traffic Violation Enforcement, Stolen Vehicle Recovery to Electronic Toll Collection.

# 6. Future Enhancements
Future work can involve fine-tuning the model to handle variations in lighting, weather conditions, image quality. Current models might struggle if multiple vehicles are captured in an image. Future models can be designed to detect and recognize multiple license plates simultaneously. Furthermore, continuous model updates and improvements can be made based on user feedback and emerging technologies in the field of object detection and computer vision.

# Web App Samples:
![1](https://github.com/user-attachments/assets/fee1679b-7c6d-4e62-aee6-3bdb2bd2b671)
![4](https://github.com/user-attachments/assets/1b98a437-9b5d-4d06-823b-7f9ac268e6ef)

# Metrics:
![2](https://github.com/user-attachments/assets/1dfdf3d2-c40d-46b5-8c40-bcf79723954e)
![8](https://github.com/user-attachments/assets/48340e16-a974-4365-9804-a1d25a29b68b)

# Video Sample:
https://github.com/user-attachments/assets/8e7e064c-5d2b-404e-815d-39bf897610b3

