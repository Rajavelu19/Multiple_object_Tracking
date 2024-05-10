<H1 align="center">
YOLOv9 Object Detection with DeepSORT Tracking(ID + Trails) </H1>


- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```
- Download the pre-trained YOLOv9 model weights
[yolov9](https://github.com/WongKinYiu/yolov9/releases/download/v0.1/yolov9-c.pt)

- Downloading the DeepSORT Files From The Google Drive 
```
gdown "https://drive.google.com/uc?id=11ZSZcG-bcbueXZC3rN08CM0qqX3eiHxf&confirm=t"
```
- After downloading the DeepSORT Zip file from the drive, unzip it. 

- Download sample videos from the Google Drive
```
gdown "https://drive.google.com/uc?id=115RBSjNQ_1zjvKFRsQK2zE8v8BIRrpdy&confirm=t"
gdown "https://drive.google.com/uc?id=1rjBn8Fl1E_9d0EMVtL24S9aNQOJAveR5&confirm=t"
```
```

#for detection and tracking
python detect_dual_tracking.py --weights 'yolov9-c.pt' --source 'your video.mp4' --device 0


#for detection and tracking with trails 
!python detect_dual_tracking.py --weights 'yolov9-c.pt' --source 'your video.mp4' --device 0 --draw-trails 
```

- Output file will be created in the ```working-dir/runs/detect/obj-tracking``` with original filename


