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

### Aligned_rgb, Aligned_depth and Label

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image2.png) ![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image3.png)

### Color_matched

The RGB value of the label visualization and the corresponding category relationship are as follows:

| Class_id | Class_name  |     RGB     |
| :------: | :---------: | :---------: |
| 0        | background  | 130,130,130 |
| 1        | desk        | 220,220,220 |
| 2        | hat         | 184,134, 11 |
| 3        | scarf       | 105,105,105 |
| 4        | T-shirt     | 118,238,198 |
| 5        | shirt       | 152,245,255 |
| 6        | sweater     | 255,248,220 |
| 7        | shorts      | 154,205, 50 |
| 8        | jeans       |  70,130,180 |
| 9        | towel       | 238,213,210 |
| 10       | bathrobe    | 105,139,105 |
| 11       | container-A | 142,229,238 |
| 12       | container-B | 205,201,165 |
| 13       | container-C | 245,245,220 |
| 14       | container-D | 238,221,130 |

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image4.png)

### misAligned

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image5.png) ![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image6.png)

### train_id and val_id

We have divided the training set and validation set of the dataset and provided the corresponding id numbers in these two files.

|        Set        |  Scale  |
| :---------------: | :-----: |
|       Train       |   258   |
|        Val        |   107   |
