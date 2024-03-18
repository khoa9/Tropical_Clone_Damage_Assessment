<a name="readme-top"></a>

# Tropical Cyclone Damage Assessment Using Satellite Imagery

<!-- PROJECT OVERVIEW -->
## Project Overview

This is the project that got my team into top participants and got a certification in the EY Open Science Data Challenge 2024. 

This project focuses on the assessment of damage caused by tropical cyclones using high-resolution satellite images. The aim is to develop a machine learning model capable of identifying and categorizing damage to coastal infrastructure, including residential and commercial buildings. By automating the detection of damaged and undamaged buildings, this project contributes to efficient and rapid disaster response efforts.

This project utilizes YOLOv8 for object detection.

<!-- PROJECT LOGO -->
<br />
<div align="center">
    <img src="runs/detect/predict/Validation_Post_Event_009.jpg" alt="Logo" width="500" height="500">


  <p align="center">
    A machine learning challenge to identify damaged and undamaged buildings from satellite imagery.
    <br />
    <a href="https://github.com/khoa9/Tropical_Clone_Damage_Assessment/blob/main/Building_Object_Detection.ipynb"><strong>Explore the notebook »</strong></a>
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Methodology">Methodlogy</a></li>
    <li><a href="#Objectives">Objectives</a></li>
    <li><a href="#Tools, Frameworks & Libraries">Tools, Frameworks & Libraries</a></li>
    <li><a href="#Dataset License">Dataset License</a></li>
    <li><a href="#Getting Started">Getting Started</a></li>
  </ol>
</details>

<!-- METHODOLOGY -->
## Methodology

The workflow of this project involves several key steps:

1. **Data Collection**: Utilize high-resolution pre- and post-event satellite imagery from sources like Maxar GeoEye-1, as well as moderate-resolution images from European Sentinel-2 and Landsat satellites.
2. **Data Annotation**: Employ LabelMe, an open-source graphical image annotation tool, to manually annotate images for training the model. Annotations identify various structures as 'Undamaged Residential Building', 'Damaged Residential Building', 'Undamaged Commercial Building', and 'Damaged Commercial Building'.
3. **Model Training**: Use the YOLO (You Only Look Once) object detection model for identifying and classifying the annotated buildings in satellite images. The model is trained on the annotated dataset to detect and distinguish between damaged and undamaged infrastructure.
4. **Evaluation and Improvement**: Assess the model's performance and iteratively refine the approach to improve accuracy and reliability in detecting and classifying building damage.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- OBJECTIVES -->
## Objectives

The primary objectives of this project include:

- **Rapid Damage Assessment**: Enable faster assessment of infrastructure damage following tropical cyclones to aid in timely disaster response and recovery efforts.
- **Automated Analysis**: Reduce the reliance on manual analysis of satellite imagery, thereby increasing the speed and scale at which damage assessments can be conducted.
- **Accuracy and Precision**: Develop a model that not only identifies damaged structures but also categorizes them with high accuracy, providing valuable insights for disaster response teams.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- TOOLS, FRAMEWORKS & LIBRARIES -->
## Tools, Frameworks & Libraries

- **[LabelMe](https://github.com/labelmeai/labelme)**: For the detailed annotation of satellite images, marking damaged and undamaged buildings.
- **[Ultralytics YOLOv8](https://docs.ultralytics.com/)**: Employed for its efficiency and accuracy in real-time object detection, YOLOv8 is used to train and validate the machine learning model on the annotated dataset.
- **Other Frameworks and Libraries:**

    * [OpenCV](https://opencv.org/)
    * [LabelMe2Yolo](https://pypi.org/project/labelme2yolo/)
    * [Rasterio](https://rasterio.readthedocs.io/)
    * [GDAL](https://gdal.org/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- DATASET LICENSE -->
## Dataset License

The dataset used in this project is provided by EY and is subject to specific licensing conditions. The data, including high-resolution satellite images and annotations, remains the property of EY. Users of this dataset are required to adhere to the terms of use specified by EY, which includes restrictions on redistribution and commercial use. For more detailed information on the licensing terms, please contact EY directly.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

To replicate the demonstration or build upon it, follow the below steps:

### Prerequisites

Installation of necessary packages:

```sh
pip install ultralytics
pip install opencv-python-headless
pip install labelme2yolo
pip install rasterio
pip install GDAL
```
### USAGE 
For detailed examples on how to use the project, refer to the Jupyter Notebook included in the repository. Additionally, consult the Ultralytics Documentation for advanced usage of YOLOv8.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONCLUSION -->
## Conclusion

This project aims to harness the power of machine learning and satellite imagery for the critical task of assessing damage following tropical cyclones. By leveraging advanced tools like LabelMe for annotation and YOLO for object detection, we strive to create a model that can significantly improve disaster response strategies through rapid and accurate damage assessment.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

