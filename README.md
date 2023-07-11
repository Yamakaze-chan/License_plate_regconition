# License_plate_regconition
This is just a simple project.   
First use HaarCascade (cv2.Cascade) to get the license plate. Then use simple CNN for character segmentation.   
CNN architecture:   
model.add(Conv2D(32, (24,24), input_shape=(28, 28, 3), activation='relu', padding='same'))   
model.add(MaxPooling2D(pool_size=(2, 2)))   
model.add(Dropout(0.4))   
model.add(Flatten())   
model.add(Dense(128, activation='relu'))   
model.add(Dense(36, activation='softmax'))   
Source Github: https://github.com/saswat0/License-Plate-Recognition/tree/master   
Dataset: 
