# easy-camera-opencv
 Easily take external camera input with configurations
# How to use
```python
# Create an object to allow for configuration
cam = Camera("./go/to/a/directory/")
# Tell it to record: object.record(seconds, 'filename', fps, height, width)
cam.record(5, 'filenameWithoutExtenstion', 30, 640, 480)
# Disconnects the external camera from the software if needed. 
cam.disconnectCamera()
```
Thats it!
# Things to know
* If there is a problem with your code, its probably opencv2 to be honest.
* Outputs .avi
* Uses XVID codec
* Record defaults to  30 fps
* Record defaults to Height: 640 Width: 480

# Whats coming
* Switching cameras
* More configurations
