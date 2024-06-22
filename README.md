# Metal Surface Defect Detection using YOLOv5 and YOLOv6

## Problem Statement

This project utilizes the NEU Metal Surface Defects Database, which contains images of metal strips with four types of typical surface defects: Crack, Pinhole, Undercut, and Shrinkage. The dataset includes 1040 images and 199 samples for each defect type.

## YOLO Models Used

- **YOLOv5**: Implemented using the Ultralytics repository. [YOLOv5 GitHub](https://github.com/ultralytics/yolov5)
  - Configuration: coco.yaml
  - Training time on T4 GPU:
    - Wall time: 43min 35s

- **YOLOv6**: Utilized from the Meituan repository. [YOLOv6 GitHub](https://github.com/meituan/YOLOv6)
  - Configuration: dataset.yaml
  - Training time on T4 GPU:
    - Wall time: 30min 38s

## Annotation Process

Data annotation was performed using [makesense.ai](https://www.makesense.ai/), a platform for image annotation.

## Project Steps

1. **Data Augmentation**: Techniques applied to enhance the diversity and quality of the training dataset.
   
2. **Data Annotation**: Annotated images to label the four types of surface defects (Crack, Pinhole, Undercut, Shrinkage).

3. **Dataset Preparation**:
   - Split the dataset into training and validation sets.
   - Organized labels and images accordingly for training.

4. **Model Training**:
   - Selected either YOLOv5 or YOLOv6 for training based on specific requirements.
   - Fine-tuned the chosen model using the annotated dataset.

5. **Testing and Evaluation**:
   - Evaluated the trained model's performance on test datasets.
   - Assessed metrics such as accuracy, precision, recall, and IoU (Intersection over Union).

## Files Included

- `Metal_Detection.ipynb`: Jupyter notebook detailing the steps for cloning and setting up YOLOv5 or YOLOv6.
- Sample images and annotations are provided in the dataset.

