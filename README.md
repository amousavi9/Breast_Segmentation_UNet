<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/ultrasound_scan.png" width="750" height="400" />
</p>

<h1 align="center">Breast-Segmentation-UNet</h1>

A breast ultrasound scan is a test that uses high frequency sound waves to create a picture of the inside of the breast. The transducer is moved over the skin of the breast to create a picture that can be seen on a computer screen. Cancers are usually seen as masses that are slightly darker (“hypoechoic”) relative to the lighter gray fat or white (fibrous) breast tissue.   
Using U-net, I will identify the area containing the tumor growth (which is not easily detectable by viewing real medical images) and compare it to the mask images. U-net architecture can localize the area of interest. It was first used in Biomedical imaging. The reason it is able to distinguish and localize the area is by classifying every pixel in the input image. So the size of input and output images is the same.   
For this project, I using Breast Ultrasound Images Dataset from kaggle. The data include breast ultrasound images among women in ages between 25 and 75 years old. This data was collected in 2018. The number of patients is 600 female patients.    
sample of Dataset. An original image of malignant tumor and contour mask (white area):
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/sample.png" width="750" height="400" />
</p>
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/img-mask.png" width="750" height="400" />
</p>

# Results
one of the biggest criticisms of deep learning and deep neural networks is that they operate as black boxes. it's hard to know exactly why a deep neural network makes a given prediction. **GradCAM** class activation visualization algorithm is one of the first steps towards interpretability at least with this algorithm we can get a sense of what regions of an image the model or the convolutional neural network is looking at in order to make a prediction and this is done by seeing which individual regions have the highest class activation as you extract a layer from the convolutional neural network and see which parts of it have the highest values and you can also inspect the direction of the gradients and the magnitude of the gradients to see which regions of the image that have been processed are now accounting for the most gradients and the most updates to the neural network. I used this algorithm here.   
Finally, I tested the model using the testing set. You can see some of the results in the pictures below.  
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/res_img1.png" width="700" height="200" />
</p>
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/res_img9.png" width="700" height="200" />
</p>
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/res_img10.png" width="700" height="200" />
</p>
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/res_img5.png" width="700" height="200" />
</p>
<p align="center">
  <img src="https://github.com/amousavi9/Breast_Segmentation_UNet/blob/main/results/res_img8.png" width="700" height="200" />
</p>
