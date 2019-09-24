# easy-camera-opencv
 Easily take external camera input with configurations
# How to use
```python
# Create an object to allow for configuration
cam = Camera("./go/to/a/directory/")
# Tell it to record: object.record(seconds, 'filename')
cam.record(5, 'filenameWithoutExtenstion')
# Disconnects the external camera from the software if needed. 
cam.disconnectCamera()
```
Thats it!
# Whats coming
* Switching cameras
* More configurations
