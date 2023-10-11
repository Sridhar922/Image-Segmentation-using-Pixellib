# Image-Segmentation-using-Pixellib

PixelLib pytorch version supports python version 3.7 and above
PixelLib Pytorch version supports these versions of pytorch(1.6.0, 1.7.1,1.8.0 and 1.9.0)

### Install Pycocotools --- pip3 install pycocotools
### Install PixelLib ---  pip3 install pixellib
### tensorflow's version (2.0 - 2.4.1)

PixelLib uses five lines of python code

import pixellib
from pixellib.torchbackend.instance import instanceSegmentation
ins = instanceSegmentation()
ins.load_model("pointrend_resnet50.pkl")
ins.segmentImage("image.jpg", show_bboxes=True, output_image_name="output_image.jpg")

Line 1–4: PixelLib package was imported and we also imported the class instanceSegmentation from the the module pixellib.torchbackend.instance (importing instance segmentation class from pytorch support). We created an instance of the class and finally loaded the PointRend model we have downloaded.

Line 5: We called the function segmentImage to perform segmentation of objects in images and added the following parameters to the function:

image_path: This is the path to the image to be segmented.
show_bbox: This is an optional parameter to show the segmented results with bounding boxes.
output_image_name: This is the name of the saved segmented image. 

# Load Model:-
Mask R CNN 2.0 file link (https://github.com/matterport/Mask_RCNN/releases/tag/v2.0)
Pointrend_resnet (https://github.com/ayoolaolafenwa/PixelLib/releases/download/0.2.0/pointrend_resnet50.pkl)
