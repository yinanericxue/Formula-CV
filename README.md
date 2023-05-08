# Formula-CV

# Object Detection = identifying multiple objects per image, and then determine their locations and classify them.

# The naive approach to doing this is to scan an image with a sliding window and feed every part of this image to a classifier. This process is very slow and will never be used for real time cases. An improved version foer this idea is the Region-based Convolutional Neural Network (R-CNN), which strategically selects regions to run through the classifier.

# YOLO stands for "you only look once" since it processes an entire image at once into a CNN. and this neural network predicts the labels, bounding boxes, and confidence probabilities for objects in the image.
![Screen Shot 2023-05-07 at 6 08 42 PM](https://user-images.githubusercontent.com/102645083/236713070-eab229d3-486d-4efd-bca3-cba5b67523a2.png)

# The first step of YOLO is to divide an image into sells with an S x S grid.
![Screen Shot 2023-05-07 at 6 14 54 PM](https://user-images.githubusercontent.com/102645083/236713544-f8c76a5e-590b-419f-849c-46c3657a002d.png)


# The next step is for each cell to predict B bounding boxes. It's okay for a small section of a bounding box to be in another cell.
![Screen Shot 2023-05-07 at 6 11 49 PM](https://user-images.githubusercontent.com/102645083/236713296-5ac24f5a-19d1-400f-8c86-cac88971af4b.png)

# The next step is to return all the bounding boxes above the confidence threshold (say 0.90).
![Screen Shot 2023-05-07 at 6 13 38 PM](https://user-images.githubusercontent.com/102645083/236713446-f62ea850-bdf2-4ccc-8f90-2426bb7050ea.png)

# It's important to note that in practice, we want larger S and B values to identify more objects.
