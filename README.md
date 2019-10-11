# easy-camera-opencv
 Easily take external camera input with configurations
# How to use
```python
# Create an object (NOTE: It will build a directory path for you if it doesn't exist)
cam = Camera("./go/to/a/directory/")

# Record for 5 Seconds to a named file
cam.record(5, 'filenameWithoutExtenstion')
# Or to use specifics: object.record(seconds, 'filename', fps, height, width)
cam.record(5, 'filenameWithoutExtenstion', 30, 640, 480) 

# Disconnects the external camera from the software if needed. 
cam.disconnectCamera()
# Switch to a different camera (NOTE: uses the same Camera object). 
cam.switchCamera(some_sort_of_cv2.VideoCapture_parameter)
```
Thats it!
# Things to know
* If there is a problem with your code, its probably opencv2 to be honest.
* Outputs .avi
* Uses XVID codec
* Recording FPS defaults to what cv2 gets as a default from your camera
* Recording resolution defaults to what cv2 gets as a default from your camera


# Whats coming
* More configurations
