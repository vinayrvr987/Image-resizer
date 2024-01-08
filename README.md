# Image-resizer
Image resizer is a project using opencv

code demonstrates how to read an image using OpenCV (cv2.imread()), resize it to different dimensions using different interpolation methods, and display the original and resized images using matplotlib.pyplot.

Here's a breakdown of the code:

Import Libraries:

cv2: OpenCV library for image processing.
numpy: Library for numerical operations.
matplotlib.pyplot: Library for plotting and displaying images.
Reading the Image:

cv2.imread(): Reads the image from the specified path ("D:\sims\eb\sim21\EB-ML-06-10-2022-Test-Output-15\PERFORATION\Overkill\Fail\Blister 1 2022-03-12 12-59-43.859 T0 M0 G0 3 PERFORATION Mono.bmp" in this case).
Resizing the Image:

cv2.resize(): Resizes the image to different dimensions and interpolation methods.
half: Resizes the image to 10% of its original size (fx = 0.1, fy = 0.1).
bigger: Resizes the image to a fixed size of 1050x1610 pixels.
stretch_near: Resizes the image to 780x540 pixels using linear interpolation (cv2.INTER_LINEAR).
Preparing Titles and Images:

Creates titles for different images: "Original", "Half", "Bigger", "Interpolation Nearest".
Stores images (original and resized) in a list.
Displaying Images Using Matplotlib:

plt.subplot(): Creates subplots to display multiple images.
Loops through the images and titles, then displays them in a 2x2 grid using plt.imshow().
Showing the Plot:

plt.show(): Shows the plot with all the images and titles.
This code snippet uses matplotlib.pyplot to display the original image and its variations after resizing with different interpolation methods, all in a single plot with titles for each image. This helps visualize how the image appears after various resizing operations.
