# Action-Recognition
This project involves the identification of different actions from video clips where the action may or may not be performed throughout the entire duration of the video. This is done using two CNN models which are  3D-CNN and LSTM models.

 
 
This project is an identification of different actions from video clips (a sequence of 2D frames). It involves two main approaches of Single Stream Network.

 

Classes:
Data is classified into 5 classes {Diving, Jumping, Basketball, Tennis, Walking}.
  
Train Data Contains 474 videos.
Divided into:
  Class	Count
  Diving	113
  Jumping	100
  Basketball	89
  Tennis	105
  Walking	67
	
Different Shapes of Videos:
  Shape	Count
  (320.0, 240.0, 239.0)	44
  (320.0, 240.0, 201.0)	32
  (320.0, 240.0, 151.0)	15
  (320.0, 240.0, 238.0)	12
  (320.0, 240.0, 105.0)	9
  ..	..
  (320.0, 240.0, 163.0)	1
  (320.0, 240.0, 310.0)	1
  (320.0, 240.0, 88.0)	1
  (320.0, 240.0, 401.0)	1
  (320.0, 240.0, 71.0)	1

	
 

  
Test Data Contains 126 videos.
Different Shapes of Videos:
Shape	Count
(320.0, 240.0, 239.0)	11
(320.0, 240.0, 179.0)	4
(320.0, 240.0, 101.0)	4
(320.0, 240.0, 119.0)	4
(320.0, 240.0, 115.0)	3
..	
(320.0, 214.0, 177.0)	1
(320.0, 240.0, 176.0)	1
(320.0, 240.0, 201.0)	1
(320.0, 240.0, 130.0)	1
(320.0, 240.0, 87.0)	1


 
 
  
A Single Stream Network - One Network for Spatial information. 
Transfer Learning Model trained on Sports Data.
Input Shape: (16, 112, 112, 3)
 
Parameters:
  batch_size = 50
  no_epochs = 50
  learning_rate = 0.0001
  validation_split = 0.2
  verbosity = 1

Train on 379 samples, validate on 95 samples.

 
--- 
Parameters:
  batch_size = 50
  no_epochs = 50
  learning_rate = 0.0001
  validation_split = 0
  verbosity = 1
	
Train on all 474 samples.
  
  

A Single Stream Network - One Network for Spatial information. 
Transfer Learning Model trained on ImageNet data.
Input Shape: (16, 112, 112, 3)

 
Parameters:
  batch_size = 40
  no_epochs = 50
  learning_rate = 0.001
  validation_split = 0.2
  verbosity = 1

--- 
Parameters:
batch_size = 40
no_epochs = 50
learning_rate = 0.001
validation_split = 0
verbosity = 1
	
Train on all 474 samples.
