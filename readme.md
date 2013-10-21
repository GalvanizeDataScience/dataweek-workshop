# Introduction to Machine Learning with Python

Welcome to [Zipfian Academy's](http://zipfianacademy.com) Machine Learning workshop. Thank you for attending, we hope you enjoyed the lecture (we sure had fun presenting).  This exercise will give you hands-on experience with the concepts covered, and will help solidify your understanding of the process of data science.

### Getting Help

As always, feel free to email us about anything at all (questions, issues, concerns, feedback) at <a href="mailto:class@zipfianacademy.com">class@zipfianacademy.com</a>.  We would love to hear how you liked the class, whether the content was technical enough (or too technical), or any other topics you wish were covered.

### Next Steps

We hope you have fun with this exercise!  If you want to learn more or dive deeper into any of these subjects, we are always happy to discuss (and can talk for days about these subjects).  And if you just can't get enough of this stuff (and want a completely immersive environment), you can [apply](http://zipfiancollective.wufoo.com/forms/m7x3z9/) for our intensive data science bootcamp starting January 20th.

### Learning Python
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               
This assignment assumes a basic familiarity with Python and is intended to teach you how to leverage it for data science.  If you do not feel comfortable enough with Python (and programming in general) I recommend these (freely available) resources:

* [Think Python](http://www.greenteapress.com/thinkpython/thinkpython.pdf)
* [MIT Open Courseware: A Gentle Introduction to Programming Using Python](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-189-a-gentle-introduction-to-programming-using-python-january-iap-2008/index.htm)
* [Learn Python the Hard Way](http://learnpythonthehardway.org/book/)
* [Python Koans](https://github.com/gregmalcolm/python_koans/wiki)

## Setup and Environment

This exercise is written in an [IPython](http://ipython.org/) [notebook](http://ipython.org/notebook.html) and uses many of wonderful libraries from the scientific Python [community](http://strata.oreilly.com/2013/03/python-data-tools-just-keep-getting-better.html).  While you do not need IPython locally to complete the exercise (there are PDF and .ipynb versions of these instructions), I recommend setting it up on your computer if you plan to continue learning and playing with data.  IPython [notebooks](http://ipython.org/ipython-doc/stable/interactive/htmlnotebook.html) not only provide an interface to interactively run (and debug) code in a web browser, but also to document your file as you go along.  Below are the steps to setup a scientific Python environment on your computer to complete this (and all future class') assignment.  If you have tips or suggestions to make this process easier, please reach out either on Piazza or via email.

### Version control and Environment Isolation
* [Git](http://git-scm.com/): Distributed Version Control to keep track of changes and updates to files/data.
* [virualenv](http://www.virtualenv.org/en/latest/): Python environment isolation to help manage dependencies with packages and versions.
* [pythonbrew](https://github.com/utahta/pythonbrew): Manage and install multiple versions of Python.  Can be handy if you want to experiment with Python 3.x.

### Scientific Python packages
     
* [Enthought Python Distribution](https://www.enthought.com/products/epd/free/): A freely available packaged environment for scientific Python.
* [Scipy Superpack](http://fonnesbeck.github.io/ScipySuperpack/): Only for Mac OSX, but a one line shell script that installs all the fundamental scientific computing packages.
* [pandas](http://pandas.pydata.org/): Data analysis and statistical library providing functionality in Python similar to [R](http://www.r-project.org/).

<em>if you are on OSX, you may need to install [Xcode](http://developer.apple.com/library/ios/#documentation/DeveloperTools/Conceptual/WhatsNewXcode/Articles/xcode_4_3.html) (with command line utilities) or install [gcc](https://medium.com/kr-projects/6e54e8c50dc8) directly</em>
   
__[Tutorial](https://sites.google.com/site/pythonbootcamp/preparation/software) walking you through the installation of these tools, with [tests](https://sites.google.com/site/pythonbootcamp/preparation/testing-that-it-all-works) to make sure it all works.__

## User knowledge modelling
In this tutorial we will be using the [Grockit Question logs](http://www.kaggle.com/c/WhatDoYouKnow/data?grockit_all_data.zip) dataset to predict the probability of getting the next question correct.  We will also cluster the data to find similar students.  Once we know which students will perform worse than the others (classifier), we can recommend similar (clustering) students who performed well to study with.    

### Resources
* [scikit-learn tutorial](http://scikit-learn.org/stable/tutorial/index.html)
* [Kaggle: Getting started with Python for Data Science](https://www.kaggle.com/wiki/GettingStartedWithPythonForDataScience)
* [AMPlab: Machine Learning crash course (part 1)](http://ampcamp.berkeley.edu/wp-content/uploads/2012/06/ariel-kleiner-ampcamp-2012-machine-learning-part-1.pdf) 
* [AMPlab: Machine Learning crash course (part 2)](http://ampcamp.berkeley.edu/wp-content/uploads/2012/06/tamara-broderick-amp-camp-2012-algorithms-part-2-kmeans.pdf) 
* [How Khan Academy is using Machine Learning to Assess Student Mastery](http://david-hu.com/2011/11/02/how-khan-academy-is-using-machine-learning-to-assess-student-mastery.html)
* [Machine Learning with Python -- Logistic Regression](http://aimotion.blogspot.com/2011/11/machine-learning-with-python-logistic.html)
* [Evaluation: Cross Validation](http://www.autonlab.org/tutorials/overfit10.pdf)

### Outline
1. Get the Data
2. Preparation -- vectorization and feature preparation (engineering)
3. Train -- fit/build model from known labeled data
4. Test -- evaluate model with cross validation 
5. Predict -- run model on data with unknown labels

### Goals
* Understand the various stages of the ML pipeline
    * Obtain
    * Prepare
    * Train
    * Test
    * Predict
* Get experience building models with [scikit-learn](http://scikit-learn.org/stable/)
* Decision Boundaries
* Cost Function
* Logistic Regression and the sigmoid function
* Cross Validation
    * K-fold
    * Hold out
* Optimization functions
* Classification vs. Regression
* Supervised vs. Unsupervised learning
* Kmeans clustering
* Distance functions (similarity)