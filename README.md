# Biometric-using-Iris-Recognition
Iris recognition is an automated method of biometric identification that uses mathematical pattern-recognition techniques on video images of one or both of the irises of an individual's eyes, whose complex patterns are unique, stable, and can be seen from some distance.

Procedure :-
1. Load the Dataset you want to enroll using Loading_Dataset.ipynb
2. Enroll the iris using Enrolling.ipynb
3. Compare codes using Recognition.ipynb

Methedology :-

For sample pupose, used "UTIRIS V.1" dataset <br />
You can download it form (https://utiris.wordpress.com/)<br />
Below is the sample<br />
<img src="https://github.com/gearhead0909/Biometric-using-Iris-patterns/blob/master/Results/image.jpg" alt="alt text" width="500" height="300">
<br />
<br />
<br />
After importing the Image we will pre-process the image. <br />
After that we will segment the iris and pupil using Hough Transform and integro-differential <br />
<img src="https://github.com/gearhead0909/Biometric-using-Iris-patterns/blob/master/Results/Segmented.jpg" alt="alt text" width="500" height="300">
<br />
<br />
<br />
Now, we need to tranform circular iris to Cartesian cordinates
After transforming iris will look like following.
<img src="https://github.com/gearhead0909/Biometric-using-Iris-patterns/blob/master/Results/transformed_iris.jpg" alt="alt text" width="500" height="300">
<br />
<br />
<br />
Now, we will use gabor wavelet to detect features from our iris, which will be used to detect the iris for recognition pupose.<br />
Extracted features will look like below <br />
<img src="https://github.com/gearhead0909/Biometric-using-Iris-patterns/blob/master/Results/code.png" alt="alt text" width="300" height="200">
<img src="https://github.com/gearhead0909/Biometric-using-Iris-patterns/blob/master/Results/mask.png" alt="alt text" width="300" height="200">
<br />
These features will be used to recognize the iris. <br />
We will use Jaccard Index to find the similiarity.
