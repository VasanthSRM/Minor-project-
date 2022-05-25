# Minor-project-

Each folder contains “.ipynb” files stating the Name of the Model, Aim and Results. Each implementation has certain parameters which would be mentioned in the starting of the file. These files also contains GPU and environment information, to enable others to recreate these experiments. One can run each ipynb file independently.
Note 1: SELETED_VALUES folder contain ipynb file that contain the code for a particular model having all its parameters fixed. (Only these runs will be considered for finally calculating average accuracy values.)
Note 2: For few models average values have been taken but only one or two instance(s) of the run code (.ipynb file) is kept.
Note 3: You need to install 4.5 version of opencv module for all SIFT based approaches: (Running this once per session is enough)
#Req. opencv 4.5+
!pip uninstall opencv-python #for uninstalling older version
!pip install opencv-python

The proposed models are segregated in these 5 Folders:
1. SIFT + KNN:
Contains 4 folders:
1. SIFT_KNN_K_VALUE_MAX_KEY_PADDING:
	Contains optimal K value finding code for SIFT + KNN approach (using Max_key_pad).
2. SIFT_KNN_K_VALUE_MIN_KEY:
Contains optimal K value finding code for SIFT + KNN approach (using Min_key).
	3. SIFT_KNN_MAX_KEY_PADDING:
		Contains code for SIFT+KNN (Max_key_padding) for optimal k value
	4. SIFT_KNN_MIN_KEY:
		Contains code for SIFT+KNN (Min_key) for optimal k value

2. SIFT + SVM:
1.	SIFT_SVM_MAX_KEY_PADDING:
Contains code for SIFT+SVM (Max_key_padding) approach
2.	SIFT_SVM_MIN_KEY:
Contains code for SIFT+SVM (Min_key) approach



3. SIFT + ANN: 
	1. SIFT_ANN_MAX_KEY_PADDING:
		SIFT+ANN (Max_key_padding) with various learning rate and epoch combinations.
SELETED_VALUES folder contain ipynb file that contain the code for SIFT_ANN_MAX_KEY_PADDING model having all its parameters fixed. (Only these runs will be considered for finally calculating average accuracy values.)

2. SIFT_ANN_MIN_KEY:
SIFT+ANN (Min_key_padding) with various learning rate and epoch combinations.
SELETED_VALUES folder contain ipynb file that contain the code for SIFT_ANN_MIN_KEYmodel having all its parameters fixed. (Only these runs will be considered for finally calculating average accuracy values.)


4. CNN_DRAFT_SELECTION:
Contains various learning rate and epoch combinations or both CNN_DRAFT_1 and CNN_DRAFT_2. And a separate run for CNN_DRAFT_2 (Refer Report).
Folder with the name “Tests for CNN_DRAFT_2 with 2 and 3 dense layers (excl. output layer)” contains test runs to demonstrate that increasing the number of dense layer doesn’t increase the accuracy of the model significantly. (Refer model summary)
SELETED_VALUES folder contain ipynb file that contain the code for CNN_DRAFT_SELECTIONmodel having all its parameters fixed. (Only these runs will be considered for finally calculating average accuracy values.)


5. CLAHE: 
	Consists of all combinatory models:
1.	SIFT+ KNN (Min_key) using CLAHE
2.	SIFT+KNN  (Max_key_padding) using CLAHE
3.	SIFT+SVM (Min_key) using CLAHE
4.	SIFT+SVM (Max_key_padding) using CLAHE
5.	SIFT+ANN (Min_key) using CLAHE
6.	SIFT+ANN (Max_key_padding) using CLAHE
7.	CLAHE+CNN_DRAFT_2
