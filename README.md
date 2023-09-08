# Clothing-Dataset

## Introduction

Our clothing dataset contains a total of 15 classes (Background, Desk, Hat, Scarf, T-shirt, Shirt, Sweater, Shorts, Jeans, Towel, Bathrobe, Target-A, Target-B, Target-C, Target-D). We collected 365 RGB-D images at a resolution of 512 by 256 pixels for both the RGB and depth components. We also provide pixel-level annotation labels for each image, which can be used for semantic segmentation tasks. We divided the data into training and test sets consisting of 258 and 107 image pairs respectively.

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image1.png)

## Download Links

BaiDu Cloud: [https://github.com/JLU-AI-RVLab/Clothing-Dataset](https://github.com/JLU-AI-RVLab/Clothing-Dataset) Password: <br>

Google Drive: [https://github.com/JLU-AI-RVLab/Clothing-Dataset](https://github.com/JLU-AI-RVLab/Clothing-Dataset)

## Data Structure

After downloading and unzipping, the file system is as follows:
```
Clothing_Dataset
├── Aligned_rgb
    ├── .png
├── Aligned_depth
    ├── .png
├── Label
    ├── .png
├── Color_matched
    ├── .png
├── misAligned
    ├── rgb
        ├── .png
    └── depth
        └── .png
train_id.txt
val_id.txt
```

### Aligned_rgb and Aligned_depth

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image2.png) ![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image3.png)

### Color_matched

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image4.png)

### misAligned

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image5.png) ![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image6.png)

### train_id and val_id

We have divided the training set and validation set of the dataset and provided the corresponding id numbers in these two files.

|        Set        |  Scale  |
| :---------------: | :-----: |
|       Train       |   258   |
|        Val        |   107   |

