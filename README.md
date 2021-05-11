# Depth-Estimation-Of-Martian-Surface-from-ISRO-Satellite-Images
Using Pix2Pix model for image to image translation from Domain A (ISRO satellite image of Martian Surface) to Domain B (Corresponding Depth Image)

<br>
<b>Abstract</b>
</br>
Currently, the Indian Space Research Organization (ISRO) is carrying out various research projects regarding the planet Mars. Earlier, it deployed Mars orbiter in the year 2013 for collecting information which can be further used for conducting even more in-depth research about the planet’s topography, temperature, atmosphere, etc. 

One such research area that ISRO is currently focusing on is estimating the depths of various valleys, canyon systems of the Martian planet. As per the current scenario, one such method for estimating depths is using Lidar technology. 

We proposed a method where we use Generative Adversarial Networks to estimate such Depth Maps, which can be further used for creating 3D models or simulations of the surface for researching and further planning of future missions.   
</br>

<br>
<b>Data Collection</b>
</br>
For this project currently there exists no specific dataset, which consists of both the satellite images and the depth maps, hence we created our own dataset for this project. 
<br>
The dataset consists of two type of images -<br>
&emsp;1. Satellite images which were taken from ISRO’s Mars Orbiter.<br>
&emsp;2. Depth image obtained from NASA’s MOLA map.<br>

<br>
<b>Data Preprocessing</b>
</br>
o We captured 1:1 identical pair of images from Isro satellite images and Nasa's Mola Depth Map respectively, along Valles Marineris canyon system at the map scale of 53km .<br>
<br>
o A total of 38 images were collected which were captured by MOM at different intervals of time in its orbits. <br>
o Each image was augmented to a set of 10 images thus reaching a total count of 380 images.<br>
o Different augmentation techniques were used such as :
&emsp;Resize
&emsp;Rotate
&emsp;Shift Scale
&emsp;Center Crop
&emsp;Horizontal flip
&emsp;Vertical flip
&emsp;Blur
&emsp;Brightness
&emsp;Contrasts
&emsp;Hue Saturation 
o These images were randomly partitioned into training (343) & testing (37) .
