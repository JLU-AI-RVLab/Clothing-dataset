# Clothing-Dataset

## Introduction

Our clothing dataset contains a total of 15 classes (Background, Desk, Hat, Scarf, T-shirt, Shirt, Sweater, Shorts, Jeans, Towel, Bathrobe, Target-A, Target-B, Target-C, Target-D). We collected 365 RGB-D images at a resolution of 512 by 256 pixels for both the RGB and depth components. We also provide pixel-level annotation labels for each image, which can be used for semantic segmentation tasks. We divided the data into training and test sets consisting of 258 and 107 image pairs respectively.

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image1.png)

## Download Links

BaiDu Cloud: [https://pan.baidu.com/s/13CkW5aSp0H_DFFwoAecxMw](https://pan.baidu.com/s/13CkW5aSp0H_DFFwoAecxMw) Password: 1821 <br>

Google Drive: [https://drive.google.com/file/d/1yWlEeMy_4FZEV-IoEpDYe5JDxbffc0FY/view?usp=sharing](https://drive.google.com/file/d/1yWlEeMy_4FZEV-IoEpDYe5JDxbffc0FY/view?usp=sharing)

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

We used the Kinect camera and the corresponding SDK to obtain the aligned RGB images and depth images, and did a cropping process (final size is 512×256) to preserve the most useful area. We use LabelMe to annotate RGB images at the pixel level to obtain labels for semantic segmentation tasks.

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image2.png) ![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image3.png)

### Color_matched

We provide the labels in colored RGB form in this folder for easy visualization. The RGB value of the label visualization and the corresponding category relationship are as follows:

| Class_id | Class_name  |     RGB     |
| :------: | :---------: | :---------: |
| 0        | Background  | 130,130,130 |
| 1        | Desk        | 220,220,220 |
| 2        | Hat         | 184,134, 11 |
| 3        | Scarf       | 105,105,105 |
| 4        | T-shirt     | 118,238,198 |
| 5        | Shirt       | 152,245,255 |
| 6        | Sweater     | 255,248,220 |
| 7        | Shorts      | 154,205, 50 |
| 8        | Jeans       |  70,130,180 |
| 9        | Towel       | 238,213,210 |
| 10       | Bathrobe    | 105,139,105 |
| 11       | Target-A    | 142,229,238 |
| 12       | Target-B    | 205,201,165 |
| 13       | Target-C    | 245,245,220 |
| 14       | Target-D    | 238,221,130 |

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image4.png)

### misAligned

We also provide the original images without alignment and cropping in this folder, they have relatively better quality and can be used to extend to other tasks. The size of the RGB image is 640×360, and the size of the depth image is 512×424.

![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image5.png) ![block images](https://github.com/JLU-AI-RVLab/Clothing-dataset/blob/main/Images/image6.png)

### train_id and val_id

We have divided the training set and validation set of the dataset and provided the corresponding id numbers in these two files.

|        Set        |  Scale  |
| :---------------: | :-----: |
|       Train       |   258   |
|        Val        |   107   |
