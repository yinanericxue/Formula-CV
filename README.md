# Formula-CV

# Object Detection = identifying multiple objects per image, and then determine their locations and classify them.

# The naive approach to doing this is to scan an image with a sliding window and feed every part of this image to a classifier. This process is very slow and will never be used for real time cases. An improved version foer this idea is the Region-based Convolutional Neural Network (R-CNN), which strategically selects regions to run through the classifier.

# YOLO stands for "you only look once" since it processes an entire image at once into a CNN. and this neural network predicts the labels, bounding boxes, and confidence probabilities for objects in the image.

![Screen Shot 2023-05-07 at 6 08 42 PM](https://user-images.githubusercontent.com/102645083/236713070-eab229d3-486d-4efd-bca3-cba5b67523a2.png)

# The first step of YOLO is to divide an image into sells with an S x S grid.
![Screen Shot 2023-05-07 at 6 10 52 PM](https://user-images.githubusercontent.com/102645083/236713230-aff2556a-33ad-48cd-bb89-106fbdee5146.png)
