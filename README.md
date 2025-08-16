# Crop_and_weed_detection
we made the crop and weed detection model using YOLOV3 on agricultural image data.
![](https://github.com/MISTER-MAXIMUS/imagess/blob/main/detection.jpg)



![](https://github.com/MISTER-MAXIMUS/imagess/blob/main/detection_1.jpeg)

# Problem
Weed is unwanted thing in agriculture. Weed use the nutrients, water ,land and many more thihngs that might have gone to crops.Which result less production of required crop.Farmer often use pesticides to remove weed which also affective but some pesticide may stick with crop and may causs problem for humans.

# Data
we using our dataset uploaded on drive(https://drive.google.com/drive/folders/1jHvp7WbSacNhIZ-FvgpkItR2CYL3cH5x?usp=drive_link).
This dataset contains 1300 images of sesame crops and different types of weeds with each image labels.
Each image is a 512 X 512 color image. Labels for images are in YOLO format.

# Some images
### sesame crop
![](https://github.com/MISTER-MAXIMUS/imagess/blob/main/68747470733a2f2f7777772e676f6f676c65617069732e636f6d2f646f776e6c6f61642f73746f726167652f76312f622f6b6167676c652d757365722d636f6e74656e742f6f2f696e626f78253246333734353238302532466266383636393437326361373739613336.jpeg)
![](https://github.com/MISTER-MAXIMUS/imagess/blob/main/68747470733a2f2f7777772e676f6f676c65617069732e636f6d2f646f776e6c6f61642f73746f726167652f76312f622f6b6167676c652d757365722d636f6e74656e742f6f2f696e626f78253246333734353238302532466464383465313063643536633734353136.jpeg)

### weed
![](https://github.com/MISTER-MAXIMUS/imagess/blob/main/68747470733a2f2f7777772e676f6f676c65617069732e636f6d2f646f776e6c6f61642f73746f726167652f76312f622f6b6167676c652d757365722d636f6e74656e742f6f2f696e626f78253246333734353238302532463232336531616531626332623264393736.jpeg)
![](https://github.com/MISTER-MAXIMUS/imagess/blob/main/68747470733a2f2f7777772e676f6f676c65617069732e636f6d2f646f776e6c6f61642f73746f726167652f76312f622f6b6167676c652d757365722d636f6e74656e742f6f2f696e626f78253246333734353238302532466563313264626166626634623562366531.jpeg)
![]


  
  # How to use this repo?

  This Repository is diveded in two part:-

    1. Training 
    2. Performig detection using pre train model
        - Using pytorch
        - Using openCV (skip installation using requirements.txt file)


## Training:-
 
 * For traning you have to make **Agriculture** folder on your google drive, open clone repo and copy all files from `Crop_weed_detection_training` folder and paste it in google drive.

 * Now from drive open crop_weed_detection.ipynb file and you will get all documentation regarding it within the file.


### setting up environment:-

 * First of all you need anaconda, if you don't have click here for [Download](https://www.anaconda.com/products/individual) and install.

    * Now open Anaconda Prompt and clone this repo
   ```
   (base) C:\Users\user> git clone https://github.com/MISTER-MAXIMUS/Crop-and-Weed-Detection-System.git
    ```  
     - (Optional) If you get any error like **git is not recogize internal command** than run below command
          ```
            (base) C:\Users\user> pip install git
          ``` 
      
    * change your working directory to clone repo.
      ```
      (base) C:\Users\user>cd Crop_and_weed_detection
      ```
    * After that you have to create environment to install require libraries. Follow the steps:-
       1. open Anaconda Prompt and write below command for install requirements.
           ```
            (base) C:\Users\user\Crop_and_weed_detection> conda create -n pytorchenv python=3.7.7
           ```
      2. After creating environment you have to activate it.
          ```
          (base) C:\Users\user\Crop_and_weed_detection> conda activate pytorchenv
         ```
      3.  Now run below command for install libraries
          ```
          (pytorchenv) C:\Users\user\Crop_and_weed_detection> pip install -r requirements.txt 
          ```
   * Now your environment is ready to roar:)
   
   * For detection you need weights for network. Due to large file i attaching google drive link. You have to download weight file unless you have your own weights file. [click here](https://drive.google.com/open?id=1-Aam2D-fqnwecbeHwa4rtzxtNjwcDkP6)

   
   * You have to add weights flie into `Crop_and_weed_detection > performing_detection > data > weights` folder.

## Performig detection using pre-trained model
### Using pytorch
   * Let Open jupyter lab

      ```
     (pytorchenv) C:\Users\user\Crop_and_weed_detection>jupyter-lab
     ```
 




### Using OpenCV:-

  * This easy compare to pytorch implementation and for this you don't need pytorch.

  * if you have opencv library already installed (opencv included in requirements.txt), skip this step else run below code
    ```
    pip install opencv-python
    ```
  
 
If you have any doubts feel free to ask any quesion at any time:)  
  * LinkedIn:https://www.linkedin.com/in/raj-bhushan-489632265/  
 # Thank You:) 




  




