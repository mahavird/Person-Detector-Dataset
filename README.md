# Person-Detector-Dataset

I have created this custom datset from the <b> "Penn-Fudan Database for Pedestrian Detection and Segmentation"</b> . The original datset can be found at https://www.cis.upenn.edu/~jshi/ped_html/

The dataset in the current repository has been used to train my own Person Detector with [TensorFlow's Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection).In total, there are 170 images (153 are used for training and 17 for validation).

## Getting Started

##### Folder Structure:
```
+ annotations: contains the xml files in PASCAL VOC format
+ data: contains the input file for the TF object detection API and the label files (csv)
+ images: contains the image data in jpg format
+ training: contains the pipeline configuration file, frozen model and labelmap
- a few handy scripts: generate_tfrecord.py is used to generate the input files
for the TF API and xml_to_csv.py is used to convert the xml files into one csv
- a few jupyter notebooks: draw boxes is used to plot some of the data and
split labels is used to split the full labels into train and test labels
```

## Copyright

See [LICENSE](LICENSE) for details.
Copyright (c) 2017 [Mahavir Dwivedi](http://www.mahavirdwivedi.com/).
