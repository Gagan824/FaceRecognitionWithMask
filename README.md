# FaceRecognitionWithMask

## This project is to save the images of the peoples, dosn't matter whether person is wearing mask or not. And then it will detect that person live in the live video cam.

### Steps:

step1. First run the file Image Collection.ipynb. to shoot and save the mask images and to label the mask in the images.

step2. Then run the setupAndInstallApi.ipynb. 

step 2.1 : Here it will first create working director for tensorflow object detection api and then download the model from the model zoo.

step 2.2 : Then it will create the label file

step 2.3 : Then it will create the record file for the mask images.

step 2.4 : Then it will read the config file and also will write some values to config file like model name, train and test directory etc..

step 2.5 : Then it will train the model on the images using its record file.

step 2.4 : Then it will vcreate the checkpoint.

step 2.5 : Then using the latest checkpoint it will detect the mask in the image.

step 2.6 : Then it will ask you for a person pic to save it 

step 2.7 : After that it will check the mask in the images if no mask will be there then it will store complete face image and if mask will be there then it will store the upper 
half of the face image.

step 2.8 : There are two models which will extract the features from the stored images and for the frame in the video 
#### Detect_person: it is detecting the person based on the cosine similarity between the features of stored images and frame features.
#### Detect_person_model: it is detecting the person based on the guassian classification which will classify the face in the frame.



Final output will be like : output.mp4
  
