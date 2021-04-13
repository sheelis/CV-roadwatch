# Computer Vision Road Watcher with OpenCV and Python

The goal is to use any camera stream to extract objects (such as licence plates, faces, cars, etc) from live streams of commonly available devices.

## Installation

1. Download and save the server script ```CV-roadwatch.py``` on your hard drive of a connected computer (which will act as the camera server)
2. Power on and connect your cameras:
   - [x] USB camera or built-in webcam
   - [ ] Android phone with a streaming app
   - [ ] IP camera
   - [ ] webcam with http interface?
3. Open ```CV-roadwatch.py``` in text editor and edit your camera settings (ip and usb addresses)
4. Run ```CV-roadwatch.py```

Tips

- You might want to set static IP addresses for all cameras and the server on your local network so that you don't need to change the settings again.
- Currently networked cameras do not work reliably. 
- add the server script to start up with your computer

## Usage and data flow

1. Camera records and streams live to the server (laptop etc)
2. Server analyzes and extracts requested data from video stream
3. Server logs results with timestamps and captures for each detected object on each camera
4. Server might provide lookup with official licence plate [registries](https://www.carjam.co.nz/car/?plate=HBE812)
5. Server might send an alert to every device on our network on a condition


## Helpful info and inspiration

- https://stackoverflow.com/questions/40906970/how-can-extract-text-from-video-stream
- https://www.pyimagesearch.com/2018/08/20/opencv-text-detection-east-text-detector/
- https://www.youtube.com/watch?v=fJcl6Gw1D8k
- https://www.youtube.com/watch?v=CTbMUrJ9ztQ
- https://www.youtube.com/watch?v=OBZ_daYqGdU
- https://medium.com/beesightsoft/opencv-python-connect-to-android-camera-via-rstp-9eb78e2903d5
- https://www.codespeedy.com/license-plate-recognition-using-opencv-in-python/
- https://github.com/kairess/license_plate_recognition