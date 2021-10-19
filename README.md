# Count the number of leaves present in an image

In this project I have counted the number of leaves present in an Image. The whole project was done in Python programming language on **Google Colab**. 

Throughout the project, I have used **OpenCV**'s functions to do various tasks (ie, from reading the image, pre-processing it, drawing the contours to showing the final image).

Accuracy of detection depends on the image. You will have to change some values (ie, magnify the distance transform value, change the filter size etc. depending on the size of leaves present in the image). 

## Here are the outputs of some test images on which I had ran the algorithm:

### Test case 1:
<img src="https://user-images.githubusercontent.com/51737416/137850458-65394bb6-dea3-4237-97c0-0cc6787af80e.png" width=40% height=20%>
 
### Test case 2:
<img src="https://user-images.githubusercontent.com/51737416/137849801-f195395e-aeed-4551-9e53-3386fc0f2ffb.png" width=40% height=20%>

### Test case 3:
<img src="https://user-images.githubusercontent.com/51737416/137850026-fc71ccee-1477-4bc0-81c6-423ad4913345.png" width=40% height=40%>

### Test case 4:
<img src="https://user-images.githubusercontent.com/51737416/137850361-c87a3dd0-e2f9-4bc5-b61e-c555f151cb59.png" width=60% height=60%>

## Observations:
**By observing the contours drawn on the leaves,**
- We will have to make some modifications to the values depending on the size of leaves present on the image. 
- Colour gradient changes in leaves can be an issue to detect the contours. 
- For slight overlapping of leaves, this algorithm works fine, but for large overlapping, this technique might not work as cv2.findContours() draw joint contours on overlapping objects. 
- In all other cases, the method works well when the image is placed on a less noisy background. 

## References:
### Code References:
- [OpenCV Python Documentation](https://buildmedia.readthedocs.org/media/pdf/opencv24-python-tutorials/latest/opencv24-python-tutorials.pdf)
- [Gaussian Blur](https://appdividend.com/2020/09/19/python-cv2-filtering-image-using-gaussianblur-method/)
- [Threshold](https://www.datasciencelearner.com/cv2-threshold-method-implementation-python/#:~:text=Steps%20to%20Implement%20cv2%20threshold%20in%20python%20Step,convert%20the%20color%20image%20into%20the%20grey%20image.)
- [Contours](https://docs.opencv.org/4.5.3/d4/d73/tutorial_py_contours_begin.html)

### Image References:
- [img_1.jpg](https://pt.dreamstime.com/fotos-de-stock-royalty-free-ramifique-com-as-folhas-verdes-isoladas-no-branco-image5984928)
- [img_2.jpg](https://thumbs.dreamstime.com/z/branch-green-leaves-6614593.jpg)
- [img_3.jpg](https://thumb9.shutterstock.com/image-photo/stock-photo-tea-green-leaves-watercolor-closeup-isolated-on-white-background-hand-painting-on-paper-450w-488815282.jpg)
- [img_4.jpg](https://www.absolutvision.com/files/preview/1280x966/11532319742d3djbuh8xhgaooi6h8jyarvqa1hhncmhtzwipyi7jwbztama3lm6eymsdk5j7udjrhdqyrouo8q2vsskzvm2amvf8ximqh5mxeex.jpg)


