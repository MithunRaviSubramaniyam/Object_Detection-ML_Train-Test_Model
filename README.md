# Object Detection Dataset

This project contains a custom object detection dataset prepared in YOLO format. The dataset is mainly focused on detecting safety-related objects/classes from building worker images. It includes training images, validation images, label files, class information, and a dataset configuration file that can be used for training a YOLO object detection model.

The dataset is organized into `train` and `val` folders. The `train/images` folder contains images used for model training, while `train/labels` contains the matching annotation files. The `val/images` folder contains validation images, and `val/labels` contains validation annotations. Each label file follows YOLO annotation format, where every line contains the class ID and bounding box coordinates.

The project includes a `classes.txt` file that lists the object classes and a `data_custom.yaml` file that defines the dataset paths, number of classes, and class names for YOLO training. The `download_images.py` script is used to download sample images related to building workers using the `simple_image_download` package.

This project can be used to train a custom YOLO model for object detection. To use it, install the required libraries, prepare the dataset paths correctly, and run YOLO training using the `data_custom.yaml` file. Before training, make sure the class names in `classes.txt` and `data_custom.yaml` are consistent.

The main technologies used in this project are Python, YOLO dataset format, image annotation files, and simple image downloading tools. This dataset can be improved by adding more images, increasing annotation quality, balancing the number of samples for each class, and testing the trained model on real-world images.

Before pushing this project to GitHub, update the absolute paths in `data_custom.yaml` because they currently point to a local system path. Replace them with project-relative paths so others can use the dataset easily.

Developed by Mithun Ravi.
