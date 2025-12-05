# Metal_Plane_Detection_Grasping
This project is designed for Bin-Pick task with UR Robot and Mechmind Nano Ultra scanner. 

This is an anomaly detection platform for industrial production. 

Demo and code will be released soon...

## Update
Bilibili 演示视频: [点击观看](https://www.bilibili.com/video/BV19L2VBkEBx/?spm_id_from=333.1387.upload.video_card.click&vd_source=dcc12a6fc4b4581b6a4578b624a7e6e6）

# metal plane detection & Grasping

---
## Intro.
This project is designed for Metal Plane Detection & Grasping with UR robot
### Main Fuctions:
_Detection&Grasping_
_Classification&Localization_

---

## Prerequisite
### Hardware
UR Robot
Mechmind Scanner NANO ULTRA
RobotIQ
RealSense D415
### software
VSCode
Mech-Eye-Viewer
Intel.RealSense.Viewer

---

## 1. make template
Modify OBJ in .\Classification_and_Localization\make_template.py: 
```
WS = './Classification_and_Localization'
OBJ = 'b0' 
```
```python
 python .\Classification_and_Localization\make_template.py
```
OBJ is the target object. Two templates along with 0/180 degree will be created for each OBJ, saved in ./Classification_and_Localization/templates. Each OBJ need to create one time.


## 2.Run
```
python main.py
```

Main Steps: 
Step 0: connect UR Robot
Step 1: capture data
Step 2: data preparation
Step 3: detection
Step 4: generate grasp point
Step 5: robot move (grasping)
Step 6: check metal (classcification)
Step 7: move to target place
