# Segmentation of refuge islands in high resolution arial images. Openstreet map reconciliation.

### What?
An already existing machine learning model is extended and trained for the detection of refuge islands in aerial images. Furthermore, the coordinates of these objects are extracted and prepared for comparison with the geographic database of OpenStreetMap.

### How?
The project comprises of three main phases:
- Pre-processing (dataset preparation and cleaning as wells as creation of target masks) 
- Training and testing of the model with a convolutional neural network (ResNet18 architecture)
- Post-processing ( coordinates extraction and comparison)

The code is written in Python and makes us of the Deep-Learning-Framework Fastai.

The whole data flow is visualized by the following diagram:

![Dataflow2](https://user-images.githubusercontent.com/93683895/181237595-b6ee183b-950b-4dd5-b54f-cdbc302c8450.JPG)

 # Installation for reproduction

1. Install Anaconda and Git

2. Clone the GitLab environment in the desired directory
    - open git bash or cmd
    - execute: $ git clone https://github.com/LucienOST/PT1-Refuge_Islands.git

3. Create an environment from the environment.yml file
    - open git bash in the cloned project folder (refuge-island-detection)
    - execute:  $ conda env create -f environment.yml

Activate the environment
    -execute: $ conda activate image_segmentation

Start jupyter notebook
    - execute $ jupyter notebook
