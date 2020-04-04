# PoseEstimationAutonomousDriving

## 3D object detection, i.e. estimating the absolute pose of vehicles (6 degrees of freedom i.e. 6 DoF) from a 2D image/monocular image, is a challenging task as the critical information like depth, yaw, pitch and roll are collapsed in the 2D image.
## The most popular one-stage object detection algorithms, e.g. YOLO, SSD, etc. and two-stage object detection algorithms e.g. RCNN, Mask RCNN, etc. rely on anchors to refine to the final detection location.
## Anchor based approaches are inherently slower and lack accuracy. Anchor free approach using CenterNet is accurate and fast in object detection and pose estimation as compared to anchor based approaches.
## CenterNet is evaluated here in estimating the absolute pose of vehicles from a monocular image in a real-world traffic environment. Kaggle dataset provided by Peking University and Baidu is used.
## Dataset can be found at this link : https://drive.google.com/drive/folders/1hNrrIEdAD9sNVV-zBa9KPasJy3tq3fl7

## CenterNet models with two backbones ResNet-18 and ResNeXt-50_32, codes have been upload for your reference. The performance of these models is compared. 
## We then use the information about the cars detected in the environment, to recommend a skill level (Beginner/ Medium/ Advanced) for a driver to take manual control from a hypothetical autonomous car. This determination is done based on the proximity and density of detected traffic.
## This is implemented in the 'Center_RestNet18_6Epoch_FocalLoss_with_Driver_Skill.ipynb' python notebook.
