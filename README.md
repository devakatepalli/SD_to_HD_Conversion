**SD to HD Video Resolution Converter**
This Jupyter Notebook provides a method for converting standard definition (SD) video to high definition (HD) resolution. The conversion is achieved through resizing and padding frames without using advanced diffusion models or machine learning techniques.

**Features**
Resizing: Each frame of the video is resized to a width of 640 pixels while maintaining the aspect ratio.
Padding: The resized frame is padded to fit a resolution of 1280x720 pixels, adding black borders to maintain the original aspect ratio.

**Requirements**
To run the notebook, you will need the following Python libraries:
OpenCV (cv2)
numpy
You can install these libraries using pip:
 pip install opencv-python numpy
 
**Usage**
Resizing Frames:
The width of each frame is resized to 640 pixels.
The aspect ratio of the original frame is maintained.

Padding Frames:
After resizing, each frame is padded to fit a final resolution of 1280x720 pixels.
Black borders are added to the left, right, top, and bottom as necessary.

Detailed Steps:

Calculate the new height while keeping the width fixed at 640 pixels to maintain the aspect ratio.
Use cv2.resize to resize the frame to this new dimension.
Pad the resized frame to fit a 1280x720 resolution using cv2.copyMakeBorder.

**Summary**
This notebook resizes each frame of an SD video to a fixed width (640 pixels) and then pads it to fit the target HD resolution (1280x720 pixels). This method maintains the aspect ratio of the original frames and adds black borders to fit the HD frame size. Note that this approach does not enhance image quality; it only changes the resolution.
