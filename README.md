# YOLOv4-face-mask-detection-support-for-covid19

Because of the COVID-19 pandemic of 2020, more and more people are concerned with protecting themselves using masks, that is why I created an application using OpenCV (with CUDA support) based on the YOLOv4 algorithm capable of detect people who wear the mask, not wear the mask, wear the mask but incorrect

## Dependencies:
##### YOLOV4
##### opencv with cuda
##### darknet (for webcam function or android camera function)

## How to use on webcam, android cam:

#### webcam: 
for windows: darknet.exe detector demo yolo.data yolov4-custom.cfg yolov4-custom_best.weights -c 0 thresh 0.75
for linux: darknet.exe detector demo yolo.data yolov4-custom.cfg yolov4-custom_best.weights -c 0 thresh 0.75


#### android cam:
- step 1: Download for Android phone mjpeg-stream soft: IP Webcam / Smart WebCam
  Smart WebCam - preferably: https://play.google.com/store/apps/details?id=com.acontech.android.SmartWebCam2
  IP Webcam: https://play.google.com/store/apps/details?id=com.pas.webcam
- step 2: Connect your Android phone to computer by WiFi (through a WiFi-router) or USB
- step 3: Start Smart WebCam on your phone
- step 4: Replace the address below, on shown in the phone application (Smart WebCam) and launch:
  darknet.exe detector demo yolo.data yolov4-custom.cfg yolov4-custom_best.weights http://192.168.0.80:8080/video?dummy=param.mjpg -i 0

## Some results:

# Image detection


<img src="https://user-images.githubusercontent.com/88756362/132335356-3173bdf2-2b4a-40bf-8b9a-7a8cb73e576c.jpg" width="450" height="450">
<img src="https://user-images.githubusercontent.com/88756362/132334407-311248c1-6311-4e8d-9149-cd360ee47261.jpg" width="350" height="450">

# Video detection




https://user-images.githubusercontent.com/88756362/132350056-f2af1104-42c6-48ea-8df0-3c7773fd668f.mp4



# Android Camera detection



https://user-images.githubusercontent.com/88756362/132335547-55f85662-5e21-41bd-852e-a21300aacede.mp4

