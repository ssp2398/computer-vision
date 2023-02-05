# computer-vision
Documentation
Computer vision assessment 

Objective :
         Objective 1: Count the number of rice grains in the Image.
         Objective 2: Find the number of broken grains in the image.
You can assume the following in the image:
● The background will always be blue.
● There will be a mix of broken and non-broken rice grains.
● The grains will not overlap but can touch each other.
                      

About data:
Data is available in below link 
http://shorturl.at/zHJ07 
The file will contain 2 folders train and test and a submission file.
The train folder contains 12 images with prefix:
● broken_grain_: contains only broken grains
● full_grains_: contains only full grains (non-broken grains)
● mixed_grains_: contains a mix of broken and non-broken grains.
The test folder will have 5 images on which submission needs to be made.


Techniques/methods/libraries  used:
                                 Opencv for read , importing and preprocessing image, watershad algorithms , image segmentation ,pandas for creating dataframe , numpy ,etc

Approach  for solution:
-	Importing required libraries cv2,numpy,pandas,watershad from skimage.segmentation .
-	Read the image using cv2
-	Convert image into gray shade
-	Using morphology methode removed noise from image 
-	For the touched rice grains counting apply watershad algorithm 
-	Using same method of watershad count the total number of rice grains and the broken rice grains
The challenges faced while Solving  problem:
-	Read the image in its original color format because when we try to read the image it will read in GRB format we have convert them into RGB format .
-	After read the image and converted into gray shade, I found some white dots in the images which is noise we can say , for this kind of problem I searched on some online resources then found morphology method.
-	While finding contours some of the rice grains are overlapped on each other they might be reason for wrong count of rice grains.
-	For overlapped rice grains  I applied watershad algorithm .
Other approaches for same problem statement :
                                  We can use CNN ,YOLO techniques for same computer vision problems . I didn’t used this techniques because I have only basic knowledge about those techniques. 

Thank you for going through this solution and presentations
I will try to add more approaches that came to my mind in the later in  this notebook. I found this approach more Profound, thus it is part of the solution

My Handles:
Linkedln profile: https://www.linkedin.com/in/suraj-pagade-0b54931b9  


