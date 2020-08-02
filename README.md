Open Images is a dataset of ~9M images annotated with image-level labels, object bounding boxes, object segmentation masks, visual relationships, and localized narratives. 
# 1.0 Download Your own dataset by entering the given commands in CMD or Anaconda Prompt

Step1)-- Check for your convinient dataset on https://storage.googleapis.com/openimages/web/visualizer/index.html?set=train&type=detection&c=%2Fm%2F044r5d

Step2)-- Go to--> Type--> Select Detection

Step3)-- Go to--> Options --> Deselect-- Display Boxes from all Catagory

Step4)-- Make Sure to input the same class you Searched after "--classes" in the COMMAND BELOW

Step5)-- Mention the command --limit and the number of images for each class

Step6)-- Modify Below command accordingly and Run in the directory of "OIDV4_Toolkit" where "main.py" is present

Step7)-- Type "Y" If asked for the permission "python main.py downloader --classes Frying_Pan Refrigerator --type_csv train --limit 200 "

Step8)-- After the download your dataset of Yolo wiil be present in OIDv4_Toolkit-Custom-Dataset-Collector-->OID-->Dataset-->train

Step9)-- In the downloaded repository you will get "classes.txt" Modify that with your own classes //ONE CLASS PER LINE

Step10)-- Run python "convert_annotations.py"

Your CUSTOM YOLO DATASET IS READY


# 2.0 Community Contributions
- [Denis Zuenko](https://github.com/zuenko) has added multithreading to the ToolKit and is currently working on the generalization and speeding up process of the labels creation
- [Skylion007](https://github.com/Skylion007) has improved labels creation reducing the runtime from O(nm) to O(n). That massively speeds up label generation
- [Alex March](https://github.com/hosaka) has added the limit option to the ToolKit in order to download only a maximum number of images of a certain class
- [Michael Baroody](https://github.com/mbaroody) has fixed the toolkit's visualizer for multiword classes



# Reference
"[We don't need no bounding-boxes: Training object class detectors using only human verification](https://arxiv.org/abs/1602.08405)"Papadopolous et al., CVPR 2016.

Refered from the video on Youtube Reference: https://www.youtube.com/watch?v=_4A9inxGqRM
