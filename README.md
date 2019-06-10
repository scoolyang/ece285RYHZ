# PyTorch-YOLOv3
A minimal PyTorch implementation of YOLOv3, with support for training, inference and evaluation. This file is a reversion of yolov3 and most of the py files are coming from another github author. I test and try to refrain the work. If you want to know more, please go to following github site. https://github.com/eriklindernoren/PyTorch-YOLOv3.git.

## Installation
##### Clone and install requirements
    $ git clone https://github.com/scoolyang/ece285RYHZ.git
    $ cd ece285RYHZ
    $ sudo pip3 install -r requirements.txt
    
    Except these three commend lines, user also need to use the newest vision of torchvision. 
    The easiest way is delete the original torchvision in datahub. Then use the following commend 
    to set up the newest vision of tochvision. The git hub link is showing as following.
    https://github.com/pytorch/vision.git
    
    one can install this easily.
    $ pip install torchvision

##### Download pretrained weights (Run this only if you want to train dataset.For test demo, user
don't need to type these commends)

    $ cd weights/
    $ bash download_weights.sh
    
## Train

After you finish set up environment, you can start to training. However, the first thing should do is either 
download the VOC2012 dataset from internet or generate your own dataset path as 'root' in ECE285projectTrain.ipynb. You may need to set up download as True to download the dataset. After that, just run all the files and you can see the training table show up. It may take hours to finish all the epochs.

## Test Demo

User can directly open ECE285projectTestDemo.ipynb to see the current result. However, the weights is not including in this file because it is a little bit big. The weight file's name is 'yolov3_cp_87.pth'. One should download and upload the weight file to the current folder path which is the 'ece285RYHZ' folder. During training process, one should wait about 10 minutes to wait for the dataloader to load all the test datafile. User can terminate after some time if you don't want to wait all the datasets are loading. After that user can change the number of 'plot' number to see different picture from the already loaded dataset. The download link is showing as following.
https://drive.google.com/file/d/1grTzYUMw5cDZxxS2ddqkDPj8Ex-LDFar/view?usp=sharing

    


