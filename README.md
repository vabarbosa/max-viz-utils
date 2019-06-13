# max-viz-utils

This package will allow you to quickly and easily create annotated images from predictions generated by the deep learning models of the Model Asset eXchange (MAX) in your JavaScript applications.

Currently the list of supported models includes:
- MAX Image Segmenter
- MAX Human Pose Estimator
- MAX Object Detector

## Uses

### MAX Image Segmenter
 - `getColorMap(imageData, segmentMap)`
   - this function takes an image and the corresponding segment map contained in the model payload, and returns the annotated colormap image.

### MAX Human Pose Estimator
 - `getPoseLines(imageData, poseData, colorName)`
   - this function takes an image, with the corresponding detected poses contained in the model payload, along with the name of a desired color (optionally) and returns an annotated image with drawn pose lines.


### MAX Object Detector
 - `getObjectBoxes(imageData, boxData)`
   - this function takes an image and the corresponding detected objects contained in the model payload, and returns an annotated image with drawn bounding boxes.
 - `cropObjectBoxes(imageData, boxData)`
   - this function takes an image and the corresponding detected objects contained in the model payload, and returns an array of cropped images with metadata.