# Feb/2022 Update: New driving data and annotation have been added!

* Added 1708 frames of clearly labeled thermal images. (under driving_data)
* Labeling format in PASCAL VOC. (under driving_annotation)
* Covered a highway and a local driving scenario.
* Covered four object classes including vehicles, pedestrians, small animals(dogs), and bicycles.



# An Dog Expansion Pack for The FREE FLIR Thermal Dataset
This expansion pack is prepared specifically for training a YOU-ONLY-LOOK-ONCE(YOLO) network. All frames are labeled in the YOLO format.
If you want to use this expansion pack for other purposes, images are still available for download but requires manual labeling.

The **FREE FLIR Thermal Dataset for Algorithm Training** can be downloaded [here](https://www.flir.ca/oem/adas/adas-dataset-form/).

The YOLO format has the shape of <br />
**0 0.477734 0.545833 0.077344 0.175000**<br />
* The first integer **0** represents the object class.
* The float numbers represent x, y, width, and height. 

A detailed description of the YOLO format can be found [here](https://github.com/AlexeyAB/Yolo_mark/issues/60).

FLIR's dataset includes 240 **Dog** bounding boxes. Training a learning algorithm using FLIR's dataset usually yields poor mAP on the dog class.<br />
The following are the results from training a YOU-ONLY-LOOK-ONCE(YOLOv4) network using FLIR's dataset.

mAP@IoU=50 for **Dog** is 0.00%.<br />
![yolo result](./misc/3.JPG?raw=true)

mAP@IoU=75 for **Dog** is 0.00%.<br />
![yolo result](./misc/4.JPG?raw=true)

The generated bounding boxes are
![yolo box](./misc/2.jpg)
![yolo box](./misc/1.jpg)

**The dogs are either missed or misclassified.**


## Some Highlights of This Expansion Pack
An example of the images in this expansion pack<br />
![image_example](./misc/FLIR_08863.jpeg?raw=true)

An example of the new added dog bounding box (For demonstration purposes, box for other classes are not shown in the image, but they will appear in the annotation)<br />
![image_example_ann](./misc/FLIR_08863_ann.jpeg?raw=true)

An example of the annotation <br />
**3 0.476953 0.543750 0.077344 0.170833**

* Added 3,054 more annotated frames contain **Dog** captured by a **FLIR A65 IR Temperature Sensor**.
* Including long-fur and short-fur dogs with unique heat signature.
* All frames are of **640*512** and in `.jpeg` format making it consistent with the original FLIR dataset.
* All frames are 24-bit color images.

Images are taken from a recording session, so similar frames do exist. Omit them at your own demand.



