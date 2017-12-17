# Semantic Segmentation
### Introduction
In this project, I have labeled the pixels of a road in images using a Fully Convolutional Network (FCN) programmed in Python 3.6, Tensorflow GPU 1.4, CUDA 8.0 running in AMI x4large server.

The network uses the FCN architecture described in [Long et al.](https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf)
and is trained on the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php)

I have experimented with multiple epochs, batch size, learning rates and dropouts hyper parameters during training. The final parameters are settled on the following values:

- Epochs: 50
- Batch size: 8
- Learning rate: 1e-3
- Dropout: 0.2

[//]: # (Image References)
[image1]: ./runs/1513451298.3180733/um_000014.png
[image2]: ./runs/1513451298.3180733/um_000061.png
[image3]: ./runs/1513451298.3180733/umm_000032.png
[image4]: ./runs/1513451298.3180733/umm_000077.png
[image5]: ./runs/1513451298.3180733/uu_000006.png
[image5]: ./runs/1513451298.3180733/uu_000082.png

The inference image results are stored in the runs directory.

Some of the results are shown below:

![sample][image1]

![sample][image2]

![sample][image3]

![sample][image4]

![sample][image5]

![sample][image6]

### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

### Start
##### Implement
Implement the code in the `main.py` module indicated by the "TODO" comments.
The comments indicated with "OPTIONAL" tag are not required to complete.
##### Run
Run the following command to run the project:
```
python main.py
```
**Note** If running this in Jupyter Notebook system messages, such as those regarding test status, may appear in the terminal rather than the notebook.

### Submission
1. Ensure you've passed all the unit tests.
2. Ensure you pass all points on [the rubric](https://review.udacity.com/#!/rubrics/989/view).
3. Submit the following in a zip file.
 - `helper.py`
 - `main.py`
 - `project_tests.py`
 - Newest inference images from `runs` folder  (**all images from the most recent run**)
 
 ## How to write a README
A well written README file can enhance your project and portfolio.  Develop your abilities to create professional README files by completing [this free course](https://www.udacity.com/course/writing-readmes--ud777).
