# Project 5: Capstone Project
## Deep Learning Track
### Building a Live Camera App

The **Deep Learning Track** Capstone Project is part of a number of suggested areas of research for the final project of the Machine Learning Engineer Nanodegree. Below you will find a pre-constructed project which you may use to satisfy the Capstone Project requirement. The included resources are non-exhaustive and you are free to pursue your own research beyond what is provided. Before you begin, be sure that you are familiar with the [Capstone Project rubric](https://review.udacity.com/#!/rubrics/108/view), the [Capstone Project description](https://github.com/udacity/Project-Descriptions-for-Review/blob/master/Machine-Learning/Capstone%20Project/Capstone%20Project.md), and the [project report template](https://github.com/udacity/machine-learning/blob/master/projects/capstone/project_report_template.md). These resources will be necessary to complete the Capstone Project, regardless of which domain or problem you choose to work on.

### Project Description
The objective of this project is to build a live camera app that can interpret number strings in real-world images. You will train a model that can decode sequences of digits from natural images, and create an app that prints the numbers it sees in real time. You may choose to implement your project as a simple Python script, a web app/service, or an Android app. The following is an example of an Android app:

![App](http://i.imgur.com/4efd886.png)

### Project Setup
Recommended setup for a simple Python script or web app/service:
- Python
- Numpy, SciPy, iPython
- [TensorFlow](https://www.tensorflow.org/)
- (Optional) OpenCV / SimpleCV / Pygame (to capture camera images)

(Optional) For deploying the model in an Android app:
- Android SDK & NDK (see this [README](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/examples/android/README.md))

### Tasks
Use the following instructions as a guideline to work on your project.

**Step 1: Design and test a model architecture that can identify sequences of digits in an image.**

Design and implement a deep learning model that learns to recognize sequences of digits. Train it using synthetic data first (recommended) or directly use real-world data (see step 2). There are various aspects to consider when thinking about this problem:
- Your model can be derived from a deep neural net or a convolutional network.
- You could experiment sharing or not the weights between the softmax classifiers.
- You can also use a recurrent network in your deep neural net to replace the classification layers and directly emit the sequence of digits one-at-a-time.

To help you develop your model, the simplest path is likely to generate a synthetic dataset by concatenating character images from [notMNIST](http://yaroslavvb.blogspot.com/2011/09/notmnist-dataset.html) or [MNIST.](http://yann.lecun.com/exdb/mnist/) This can provide you with a quick way to run experiments. (Or you can go directly to the real-world dataset of Step 2.) In order to produce a synthetic sequence of digits for testing, you can for example limit yourself to sequences up to five digits, and use five classifiers on top of your deep network. You would have to incorporate an additional ?blank? character to account for shorter number sequences.

Here is for example a [published baseline model](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42241.pdf) on this problem ([video](https://www.youtube.com/watch?v=vGPI_JvLoN0)).

- *What approach did you take in coming up with a solution to this problem?*
- *What does your final architecture look like? (Type of model, layers, sizes, connectivity, etc.)*
- *How did you train your model? Did you generate a synthetic dataset (if so, explain how)?*

**Step 2: Train a model on a realistic dataset.**

Once you have settled on a good architecture, you can train your model on real data. In particular, [the SVHN dataset](http://ufldl.stanford.edu/housenumbers/) is a good large scale dataset collected from house numbers in Google Street View. Training on this more challenging dataset, where the digits are not neatly lined-up and have various skews, fonts and colors, likely means you have to do some hyperparameter exploration to do well.

- *How does your model perform on a realistic dataset?*
- *What changes did you have to make, if any?*

**Step 3 (optional): Put the model into an Android app.**

Do this step only if you have access to an Android device. If you don?t, you may either:
- Take pictures of numbers that you find around you, and run them through your classifier on your computer to produce example results, or,
- Use OpenCV / SimpleCV / Pygame to capture live images from a webcam.

Loading a TensorFlow model into a camera app on Android is demonstrated in the [TensorFlow Android demo app](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/examples/android), which you can simply modify.

- *Is your model able to perform equally well on captured pictures or a live camera stream? Document how you built the interface to your model.*

**Step 4: Explore!**

There are many things you can do once you have the basic classifier in place. One example would be to also localize where the numbers are on the image. The SVHN dataset provides bounding boxes that you can tune to train a localizer. Simply training a regression loss to the coordinates of the bounding box is one way to get decent localization.

Once you have the data localized, you can for example try turn it into an augmented reality app by overlaying your answer on the image like the [Word Lens](https://en.wikipedia.org/wiki/Word_Lens) app does. Those are just examples of extensions you can look into. Use your imagination!

- Make sure to report what extension(s) you have implemented and how they worked.
  
### Submitting your Project

Please refer to the [Capstone Project rubric](https://review.udacity.com/#!/rubrics/108/view) to self-evaluate your work before submitting. The following deliverables will be required as a single compressed archive:
- All of the necessary project code, datasets, supplementary files for your project
- Your project report as a PDF, which adheres to a similar structure of the [project report template](https://github.com/udacity/machine-learning/blob/master/projects/capstone/project_report_template.md)
- A README with title text **"Build a Live Camera App"** along with instructions about running the code and acquiring datasets (if necessary).

### Available Courses 

- [Deep Learning](https://www.udacity.com/course/deep-learning--ud730) (Google and Udacity)

### Relevant Sources
- Goodfellow, I., Bengio, Y. and Courville, A. *[Deep Learning](http://www.deeplearningbook.org/)*. MIT Press, 2016
- Netzer, Y., et al. [Reading Digits in Natural Images with Unsupervised Feature Learning](http://ufldl.stanford.edu/housenumbers/nips2011_housenumbers.pdf). *NIPS Workshop on Deep Learning and Unsupervised Feature Learning*, 2011.
- Goodfell, I., et al. [Multi-digit Number Recognition from Street View Imagery using Deep Convolutional Neural Networks](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42241.pdf). *ICLR*, 2014. [[video](https://www.youtube.com/watch?v=vGPI_JvLoN0)]
- [UFLDL Deep Learning Tutorial](http://deeplearning.stanford.edu/tutorial/)
- [DeepLearning.net](http://deeplearning.net/): A collection of papers, software, datasets, and current events.
- [Deep Learning Summer School, Montreal 2015](https://sites.google.com/site/deeplearningsummerschool/).
- [Street View House Numbers (SVHN)](http://ufldl.stanford.edu/housenumbers/): A large-scale dataset of house numbers in Google Street View images.