# An Dog Expansion Pack for The FREE FLIR Thermal Dataset for Algorithm Training
This expansion pack is prepared specifically for training a YOU-ONLY-LOOK-ONCE(YOLO) network. All frames are labeled in the YOLO format.
If you want to use this expansion pack for other training, images are still available to download but requires manual labeling.

A description of the YOLO format can be found [here](https://github.com/AlexeyAB/Yolo_mark/issues/60).

The **FREE FLIR Thermal Dataset for Algorithm Training** can be found [here](https://www.flir.ca/oem/adas/adas-dataset-form/) with detailed description.

FLIR's dataset includes 240 labeled frames of **Dog**. Training an algorithm only by this dataset usually yields poor AP on the dog class.<br />
The following is the result of training a YOU-ONLY-LOOK-ONCE(YOLOv4) network using FLIR's dataset.
![yolo result](./3.JPG?raw=true)

At IoU=0.5, AP for **Dog** is 0.00%.




**Highlights of This Expansion Pack**<br />
Training a YOLO(v3/v4) network only by FLIR's dataset usually yields poor performance on dogs.

Added in more **DOG** frames captured by a **FLIR A65 IR Temperature Sensor** for increased data variety.
All frames are 24-bit of dimension **875*700**.

