# face

A place to store information on face detection , landmark detection, and angle inference tools. 

* Face detection / landmark * 

|    Name       |# LM |face |angle        | Notes |     Tested |   [ FSA-Net](https://github.com/omasaht/headpose-fsanet-pytorch) - input = image+bbox. problems with angles > 30degrees |     [6Drepnet](https://github.com/thohemp/6DRepNet) input = 68 points - not better than fsanet, but that could be due to upstream landmarks detection  |  [yinguobing](https://github.com/yinguobing/head-pose-estimation) input = 68 points |
| ------------- | ------------- |---- |---- | ------------- | ------------- |  ------------- |  ------------- | ------------- |
|  [MTCNN](https://pypi.org/project/mtcnn/)        | 5  | _   |_   |Reliable, slow  | :heavy_check_mark:   | compatible  | _   |   _   | 
|  [dlib](https://pypi.org/project/dlib/)         | 68  |_   |_   | not as good as MTCNN , dissappointing quality on angles | :heavy_check_mark:  | _   | compatible   |    _   | 
| mnssd         | 5 |_   |_   | also good (like MTCNN)  | :heavy_check_mark:  | _   | _   |  _   | 
| [yolov5-face](https://github.com/deepcam-cn/yolov5-face)   | 5  |_   |_   | Reliable  |:heavy_check_mark:  |  current best practice  | _   |  _   | 
| [yolov8-face](https://github.com/derronqi/yolov8-face)   | 5  |_   |_   | _  | _   | _   | _   |   _   | 
| [Wish yolov8face (51)](https://github.com/wish44165/Optimizing-Facial-Landmark-Estimation-for-Embedded-Systems)  | 51  |_   |_   | question wide angle?  |:heavy_check_mark:  | _   | _   |   _   | 
|  [6Drepnet](https://github.com/thohemp/6DRepNet)     | 68 | _   |_   |fastish, less reliable than yolov5-face  |:heavy_check_mark:   | _   | _   |    _   | 
| [deepface](https://pypi.org/project/deepface/#:~:text=Deepface%20is%20a%20hybrid%20face,configuration%20uses%20VGG%2DFace%20model.)  | max 5  |_   |_   |  many backbones | _  | _   | _   |    _   | 
| [face-recognition](https://pypi.org/project/face-recognition/)  | 5  |_   |_   |   many backbones   | _   | _   | _   |    _   | 
| blazeface (mediapipe)  | ?  |_   |_   | FAST, but unreliable on small faces.   | :heavy_check_mark:  | _   | _   |    _   | 
| [face_alignment](https://github.com/1adrianb/face-alignment) (adrian bulat) | 68  |_   |_   | not stable   | :heavy_check_mark:  | _   | compatible  |    :heavy_check_mark:    | 
| [yinguobing](https://github.com/yinguobing/head-pose-estimation) (pose68) | 68  | :heavy_check_mark:   | :heavy_check_mark: input = 68 2D points, uses PnP from 3D model    |large angles not good! occluded landmarks are guessed or incorrect  | :heavy_check_mark:  | _   | not tested, due to bad 68 point accuracy  | :heavy_check_mark:   | 

