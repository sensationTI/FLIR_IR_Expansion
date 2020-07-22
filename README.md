# An Dog Expansion Pack for The FREE FLIR Thermal Dataset for Algorithm Training
This expansion pack is prepared specifically for training a YOU-ONLY-LOOK-ONCE(YOLO) network. All frames are labeled in the YOLO format.
If you want to use this expansion pack for other training, images are still available for download but requires manual labeling.

The **FREE FLIR Thermal Dataset for Algorithm Training** can be downloaded [here](https://www.flir.ca/oem/adas/adas-dataset-form/).

The YOLO format has the shape of <br />
**0 0.477734 0.545833 0.077344 0.175000**<br />
* The first integer **0** represents the object class.
* The float numbers represent x, y, width, and height. 

A detailed description of the YOLO format can be found [here](https://github.com/AlexeyAB/Yolo_mark/issues/60).

FLIR's dataset includes 240 **Dog** bounding boxes. Training an algorithm only by this dataset usually yields poor AP on the dog class.<br />
The following is the result of training a YOU-ONLY-LOOK-ONCE(YOLOv4) network using FLIR's dataset.
![yolo result](./3.JPG?raw=true)

At IoU=0.5, AP for **Dog** is 0.00%.<br />
The Bounding boxes generated are
![yolo box](./2.jpg?raw=true)
![yolo box](./1.jpg?raw=true)

Dogs are either misclassified or completely missed.



**Highlights of This Expansion Pack**<br />
* Added in 3,054 more **DOG** frames captured by a **FLIR A65 IR Temperature Sensor**.
All frames are 24-bit of dimension **875*700**.

