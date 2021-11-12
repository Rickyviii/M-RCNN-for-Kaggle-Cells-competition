This repo uses computer vision MRCNN algorithm for the following kaggle competition: <br>
https://www.kaggle.com/c/sartorius-cell-instance-segmentation

M-RCNN is well designed for instance segmentation, which is required here: 

<i>(extract of Kaggle competition overview)</i><br>
"In this competition, you’ll detect and delineate distinct objects of interest in biological images depicting neuronal cell types commonly used in the study of neurological 
disorders. More specifically, you'll use phase contrast microscopy images to train and test your model for instance segmentation of neuronal cells. 
Successful models will do this with a high level of accuracy."

This repo contains my Google colab notebook, run with TensorFlow 2.3, which presents:
- a data visualisation of the training images provided
- the import of an already trained model on a CocoDataset images set, provided by Matterport (see below)
- we apply transfer learning on this model by removing its upper layers
- various training of this model with input/output Kaggle training images/data
- the results obtained, with metric calculation and graphical display

Here, we import the M-RCNN algorithm code initially provided by Matterport (TensorFlow V1 compatible only), and 
modified to make it compatible with Tensorflow 2.3. by Leekunhee.

Matterport source: https://github.com/matterport/Mask_RCNN <br>
Leekunhee Source: https://github.com/leekunhee/Mask_RCNN.git

