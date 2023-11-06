# COLOR RECOGNITION

This project focuses on color classifying by K-Nearest Neighbors Machine Learning Classifier which is trained by R, G, B Color Histogram. It can classify White, Black, Red, Green, Blue, Orange, Yellow and Violet. If you want to classify more color or improve the accuracy you should work on the [training data]
## Quick Demo

***Run [color_classification_webcam.py]to perform real-time color recognition on a webcam stream.***

<p align="center">
  <img src="https://user-images.githubusercontent.com/22610163/34917659-8497acae-f95a-11e7-93fb-f7cd6cc3128a.gif">
</p>

***Run [color_classification_image.py] to perform color recognition on a single image.***

<p align="center">
  <img src="https://user-images.githubusercontent.com/22610163/42423806-14cdfa7a-8309-11e8-9478-23d50fc0002f.png">
</p>

---
**What does this program do?**
1. **Feature Extraction:** Perform feature extraction for getting the R, G, B Color Histogram values of [training images]
2. **Training K-Nearest Neighbors Classifier:** Train KNN classifier by R, G, B Color Histogram values
3. **Classifying by Trained KNN:** Read Web Cam frame by frame, perform feature extraction on each frame and then classify the mean color of it by trained KNN classifier.
---

**TODOs:**

- "Add New Color" utility will be added.
- New feature extractors will be added.
- New classifiers will be added.


## Theory

In this study, colors are classified by using K-Neares Neşghbor Machine Learning classifier algorithm. This classifier is trained by image R, G, B Color Histogram values. The general work flow is given at the below.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22610163/35335133-a9632c70-0125-11e8-9204-0b4bfd0702a7.png" {width=35px height=350px}>
</p>

You should know 2 main pheomena to understand basic Object Detection/Recognition Systems of Computer Vision and Machine Learning.

**1.) Feature Extraction**

How to represent the interesting points we found to compare them with other interesting points (features) in the image.

**2.) Classification**

An algorithm that implements classification, especially in a concrete implementation, is known as a classifier. The term "classifier" sometimes also refers to the mathematical function, implemented by a classification algorithm, that maps input data to a category.

For this project;

**1.) Feature Extraction** = Color Histogram

Color Histogram is a representation of the distribution of colors in an image. For digital images, a color histogram represents the number of pixels that have colors in each of a fixed list of color ranges, that span the image's color space, the set of all possible colors.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22610163/34918867-44f5feaa-f96b-11e7-9994-1747846266c9.png">
</p>

**2.) Classification** = K-Nearest Neighbors Algorithm

K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions). KNN has been used in statistical estimation and pattern recognition already in the beginning of 1970’s as a non-parametric technique.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22610163/34918895-c7b94d24-f96b-11e7-87da-8619d9bd4246.png">
</p>



I think, the training data has a huge important in classification accuracy. I created my training data carefully but maybe the accuracy can be higher with more suitable training data.

Another important thing is lightning and shadows. In my test images, the images which were taken under bad lighting conditions and with shadows are classified wrong (false positives), maybe some filtering algorithm should/can be implemented before the test images send to KNN classifier Thus, accuracy can be improved.

## Citation
If you use this code for your publications, please cite it as:

    @ONLINE{cr,
        author = "Manikant Avargol",
        title  = "Color Detection",
        year   = "2020",
        url    = "(https://github.com/manikantavargol/Colour-detection)"
    }

## Author
Manikant Avargol

## License
This system is available under the MIT license. See the LICENSE file for more info.
