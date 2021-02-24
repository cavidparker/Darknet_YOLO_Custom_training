# Darknet_YOLO:
- git clone https://github.com/pjreddie/darknet
- cd darknet
- make
## Download pre-trained weight
- wget https://pjreddie.com/media/files/yolov3.weights
## Test
- ./darknet detect cfg/yolov3.cfg yolov3.weights data/dog.jpg


# Darknet_YOLO_Custom_training:
- go data folder and create two file and one folder
- 1. obj.data
- 2. obj.names
- 3. Create a folder named as (obj)

# Run generate_train.py (see the result in the data folder named train.txt

# Go to cfg folder and open yolov3-custom.cfg file and modify this:
- STEP 1 : max_batches = 
-                      1 class = 2000 but as default 4000
-                      2 class = 2000*2 = 4000
-                      3 class = 2000*3 = 6000

- STEP 2 : steps=
-                80% of max_batches and 90% of max_batches

- STEP 3 : change all 3 yolo classes(that how many classes you have)


