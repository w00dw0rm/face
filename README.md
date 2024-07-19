# face

A place to store information on face detection , landmark detection, and angle inference tools. 

* Face detection / landmark * 

|    Name       |# LM         | Notes |     Tested |
| ------------- | ------------- | ------------- | ------------- |
|  [MTCNN](https://pypi.org/project/mtcnn/)        | 5  | Reliable, slow  | :heavy_check_mark:   |
|  [dlib](https://pypi.org/project/dlib/)         | ?  | not as good as MTCNN  | :heavy_check_mark:  |
| mnssd         | 5 | also good (like MTCNN)  | :heavy_check_mark:  |
| [yolov5-face](https://github.com/deepcam-cn/yolov5-face)   | 5  | Content Cell  |:heavy_check_mark:  |
| [yolov8-face](https://github.com/derronqi/yolov8-face)   | 5  | Content Cell  | _   |
| [Wish yolov8face (51)](https://github.com/wish44165/Optimizing-Facial-Landmark-Estimation-for-Embedded-Systems)  | 51  | question wide angle?  |:heavy_check_mark:  |
|  [6Drepnet](https://github.com/thohemp/6DRepNet)     | 68 | fastish, less reliable than yolov5-face  |:heavy_check_mark:   |
| [deepface](https://pypi.org/project/deepface/#:~:text=Deepface%20is%20a%20hybrid%20face,configuration%20uses%20VGG%2DFace%20model.)  | max 5  |  many backbones | _  |
| [face-recognition](https://pypi.org/project/face-recognition/)  | 5  |   many backbones   | _   |
| blazeface (mediapipe)  | ?  | FAST, but unreliable on small faces.   | :heavy_check_mark:  |



