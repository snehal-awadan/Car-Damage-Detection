# Car damage detection project:

Developed a high-performance car damage detection model using the YOLOv8 framework for the insurance sector. Leveraged transfer learning to accelerate model training and achieve high accuracy in identifying and localizing ten distinct damage categories. Utilized a comprehensive dataset of diverse damage types to train the model. Deployed the model as a user-friendly Streamlit-based web application, streamlining insurance claims processing through efficient damage assessment.

# About dataset:

The dataset includes 9900 images.
Damage are annotated in YOLOv8 Oriented Object Detection format.

# How to start:

Step 1: Set Up Your Development Environment
Install Dependencies:
Ensure you have Python and pip installed.
Install necessary libraries: OpenCV, NumPy, and TensorFlow/Keras or PyTorch (depending on the YOLO implementation).

Get YOLO Weights and Configuration:
Download the pre-trained YOLO weights and configuration files from the official YOLO GitHub repository or other reliable sources.
For YOLOv3, download yolov3.weights, yolov3.cfg, and the coco.names file.

Step 2: Prepare Your Dataset
Collect Data:
Gather images of vehicles with various types of damage.
Annotate the images to create bounding boxes around damaged areas. You can use tools like LabelImg or VoTT for annotation.

Format Data:
Ensure your dataset is in the correct format for training YOLO. This usually involves having image files and corresponding annotation files in YOLO format.

Step 3: Set Up YOLO for Training
Modify Configuration Files:
Update the YOLO configuration file (e.g., yolov3.cfg) to match your dataset. This includes setting the number of classes, filters, and other hyperparameters.
Create a Custom Dataset Configuration File:

Create a '.data' file that specifies the paths to your training, validation, and names files.
Set Up the Training Script:
Use a training script (provided by the YOLO implementation you are using) to train the model on your custom dataset.

Step 4: Train the YOLO Model
Training:
Run the training script, specifying the paths to your dataset and configuration files.
Monitor the training process and adjust hyperparameters if necessary.

Step 5: Evaluate and Test the Model
Evaluate Performance:
After training, evaluate the model's performance on a validation set.
Check metrics like precision, recall, and MAP (mean Average Precision).

Test on New Images:
Test the trained model on new, unseen images to ensure it accurately detects vehicle damage.

Step 6: Integrate and Deploy
Create a Detection Script:
Write a script to load the trained YOLO model and run it on new images or video streams to detect vehicle damage.

