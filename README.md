# YoloV8
The model underwent training using an augmented image dataset from the video game Halo Infinite, comprising screenshots of an online gameplay session. Specifically designed for object detection, the labels indicate "enemy" and "enemy-head". The model was trained for 25 epochs, and the results are presented below. There are some signs of overfitting at first but the graph stabilized after the 10th epoch.

![download](https://github.com/ali0onder/YoloV8/assets/129281448/0c367f38-1ff5-4c3d-8178-d7b0fc040010)

Confusion matrix shows that the most predictions are accurate.

![download](https://github.com/ali0onder/YoloV8/assets/129281448/0a775942-19e8-4ff1-875f-5793de7bf032)

The overall scores:

| Class        | Box   | R     | mAP50 | mAP50-95 |
|--------------|-------|-------|-------|----------|
| all          | 0.96  | 0.893 | 0.962 | 0.711    |
| enemy        | 0.955 | 0.933 | 0.978 | 0.82     |
| enemy-head   | 0.965 | 0.853 | 0.947 | 0.602    |


The original dataset is made by Graham Doerksen. 
Dataset source: https://universe.roboflow.com/graham-doerksen/halo-infinite-angel-aim
