# Darknet_YOLO_Custom_training:
- git clone https://github.com/pjreddie/darknet
- cd darknet
- make
## Download pre-trained weight
- wget https://pjreddie.com/media/files/yolov3.weights
## Test
- ./darknet detect cfg/yolov3.cfg yolov3.weights data/dog.jpg
