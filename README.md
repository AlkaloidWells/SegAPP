# SegAPP
A Mathlab app build with math mathlab app builder for demontration of amage filtering, cleaning and segmentation 

# Digital image processing Image segmentation

Task Description:
Implementation of an optimized image segmentation tool
Segmentation is one of the most important image processing for object detection,
recognition, etc. The segmented regions have the same characteristics. But it is a complex task
and the some of the known techniques will not lead to a good accuracy. A hybrid approach of
two stages (edges detection + region growing techniques) was proposed and implemented by
Amitab et al. See the attached paper.
Here you are provided with two papers. The first paper is a review of the segmentation
techniques and the second one deals with the above-mentioned approach.
Your task is to select one edge detection techniques from the first paper and combine with
the region growing method as explained in the second; to implement a tool that successfully
segment a set of images of your choice.
Write the complete report per group of 4 students and submit before the given deadline.

Proposed Solution
A desktop application with multiple and real time image processing action, our solution comes with the ability to
a. upload images
b. add Noise effect
c. Remove noise
d. Rgb2gray
e. Dredge Detection
f. Segmentation
g. Object separation
This functionality was implemented to excise the importance of image processing specifically in the medical department. Our application was developed on mathlab using mathlab app builder.
In our solution we made use of
1. Laplacian of Gaussian
An edge detection algorithm for detecting the edges of objects in an image. useful for detecting edges that appear at various image scales or degrees of image focus. The exact values of sizes of the two kernels that are used to approximate the Laplacian of Gaussian will determine the scale of the difference image, which may appear blurry as a result.
This method is useful for detecting edges that appear at various image scales or degrees of image focus. he exact values of sizes of the two kernels that are used to approximate the Laplacian of Gaussian will determine the scale of the difference image, which may appear blurry as a result. Generally, this method has proven to be more efficient than most edge detection algorithm, that’s why we make use of this solution
2. Region Growing Region growing is a region-based sequential technique for image segmentation by assembling pixels into larger regions based on predefined seed pixels, growing criteria, and stop conditions. A segmentation technique based on the similarity of adjacent pixels.
Region is grown from the seed pixel by adding in neighboring pixels that are similar, increasing the size of the region. When the growth of one region stops, we simply choose another seed pixel which does not yet belong to any region and start again.
Here we will be applying a combination of edge cutting and region growing know as a hybrid
Functionalities

1) Upload image
To perform action on our image we need and image so wee make use of mathlab libraires for uploading path returning the image path, name and the image to GUI as seen on the figure bellow.

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/02b89dc1-d063-44c8-a855-7ea6b1236c16)

2) Noise
After uploading image users can perform cetene operation like adding noise to the image.
Noise in photography can be defined as a random variation in the image signal. Noise can be caused by a number of factors, including poor lighting conditions, high ISO settings, long exposure times, and heat. Noise can also be introduced into an image during the editing process.
The figure bellow shows been added to the image uploaded.

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/eba814e5-4fc4-462d-9e1c-a7939ed32661)

3) Removing Noise
The same as there could be noise on an image noise can be removed from an image. Removing random points or pixel from the image
![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/2cd2645e-d981-442a-959a-11a850c8b86c)

4) Rgb2gray
The rgb2gray function converts RGB images to grayscale by eliminating the hue and
saturation information while retaining the luminance. If you have Parallel Computing Toolbox™ installed, rgb2gray can perform this conversion on a GPU. example.
newmap = rgb2gray( ‘im4.png’ ) returns a grayscale colormap equivalent to map

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/94225f77-7184-4edd-a07f-ad8601d6798b)

5) Edge detection
includes a variety of mathematical methods that aim at identifying edges, curves in a digital image at which the image brightness changes sharply or, more formally, has discontinuities. The same problem of finding discontinuities in one-dimensional signals is known as step detection and the problem of finding signal discontinuities over time is known as change detection. Edge detection is a fundamental tool in image processing, machine vision and computer vision, particularly in the areas of feature detection
The image in the green box is the original image and the one in the one in the red box is the edge detected image

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/e3f09955-3cf6-4568-8d74-7f4b0c9ba6f6)

6) Segmentation Image segmentation involves converting an image into a collection of regions of pixels that are represented by a mask or a labeled image. By dividing an image into segments, you can process only the important segments of the image instead of processing the entire image.
For our segmentation we will be making use of our edge detection algorithm “LOG” and Region Growing.
The image in the green box is the original image and the one in the one in the red box is the segmented image

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/7795c79a-fd20-4705-b03f-4fc73ddf8b41)

7) Segmentation _Separation
This helps us to perform object detection finds bounding boxes around objects and classifies them. Instance segmentation adds, for every detected object, a pixel mask that gives the shape of the object.
The medical department uses this to perform analysis om specific part of MIR images by segmenting the image into different parts this is done by playing with the threshold of the individual images. In this case study we are trying to extract the largest part of the brain.
The image in the green box is the original image and the one in the one in the red box is the required object image.

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/c1be84b5-9929-4105-aedc-658eb7d06f45)

We could further arrange the image such that u could have another object just adjust the threshold by increasing or decreasing to get the object.

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/464a2f1d-299d-4d7c-885a-752a9b763ab6)

![image](https://github.com/AlkaloidWells/SegAPP/assets/55930366/568eb2e4-0aff-4e15-a758-d725f13d3398)

Conclusion
Generally, the experience was a success and contained a lot of exposure. Thu I did not meet a few of my expectations never the less image processing is necessary tool for many department
