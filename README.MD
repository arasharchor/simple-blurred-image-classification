Simple Blurred Image Classification with OpenCV in python


In this code, you can recognise those blurred images in your photo album which can contain thousands of images. 



The first argument is  --images:  the path to the directory containing our dataset of images we want to test for blurryness.

Also an optional argument --thresh has been  defined, which is the threshold we’ll use for the blurry test. If the focus measure for a given image falls below this threshold, we’ll mark the image as blurry. It’s important to note that you’ll likely have to tune this value for your own dataset of images. A value of 1300  seemed to work well for my test images, but this value is quite subjective to the contents of the image(s), so you’ll need to play with this value yourself to obtain optimal results.

Believe it or not, the hard part is done! We just need to write a bit of code to load the image from disk, compute the variance of the Laplacian, and then mark the image as blurry or non-blurry:




#To get started

1- OpenCV should be installed

2- pip intall imutils

3- Now that we have classify_blurred_Image.py  script coded up, let’s give it a shot. Open up a shell and issue the following command:

python classify_blurred_Image.py --images images


If you use this code, please don't forget to cite me: @smajida Seyed Majid Azimi
