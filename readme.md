# Project Name :Diabetic Retinopathy detection   

# Problem statement :    
Diabetic Retinopathy is a disease with an increasing prevalence and the main cause of blindness among working-age population. The risk of severe vision loss can be significantly reduced by timely diagnosis and treatment. Systematic screening for DR has been identified as a cost-effective way to save health services resources. Automatic retinal image analysis is emerging as an important screening tool for early DR detection, which can reduce the workload associated to manual grading as well as save diagnosis costs and time. Many research efforts in the last years have been devoted to developing automated tools to help in the detection and evaluation of DR lesions.
We are interested in automating this predition using deep learning models.

# Dataset : [APOTS Kaggle Blindness dataset](https://www.kaggle.com/c/aptos2019-blindness-detection)      

# Solution :   
we proposing Deep Learning classification technique using CNN pretrained model [resnet152](https://github.com/pytorch/vision/blob/master/torchvision/models/resnet.py) to classify severity levels of DR ranging from 0 (NO DR) to 4 (Proliferative DR).   
This is a collaborative project of team of three where my main work is on developing, training and testing various CNN models along with some secondary work.
Deep learning looks promising because already various types of image classification tasks has been performed by various CNN's so, we can rely on DL pretrained models or we can modify some layers if we wish to :)    
A GUI based system has been made using Tkinter and used heidiSQL to maintain and store a list of predictions with their patient username , password and predit value.   
     

# Summary of Technologies used in this project :       
| Dev Env. | Framework/ library/ languages |
| ------------- | ------------- |
| Backend development  | PyTorch (Deep learning framework) |
| Frontend development | Tkinter (Python GUI toolkit) |
| Database connectivity | HeidiSQL (MySQL server) |
| Programming Languages | Python, SQL |
    


# Resnet152 model summary :     
I have only shown below the main layers of resnet and each of the 'layer1', 'layer2', 'layer3' and 'layer4' contains various more layers.        
[https://www.kaggle.com/datasets/pytorch/resnet152]

# Getting started :
Step 1:     Collection of dataset images where images are trained and classified as (0 - No   
                DR ,1- Mild DR,2 - Moderate DR, 3 - Severe DR, 4 - Proliferative DR)
Step 2:     Image is uploaded by user
Step 3:     Image is converted from BGR format into RGB format
Step 4:     Image is cropped 
Step 5:     After cropping the image, it is converted into gray scale to resize the
                image and detect the type of stage
Step 6:     Image is classified and output is predicted which is displayed to the user based     
                 on the stage level  (0 - No DR ,1- Mild DR , 2 - Moderate DR ,3 - Severe DR ,  
                 4 - Proliferative  DR)
# Some snaps :     
In screenshots file     

 # Future Prospect :    
 * our next goal is to develop this into WebApp (probably using some light weight model as resnet models are heavy).   
 * Next goal will be using encryption techniques to achieve not only high accuracy but also high level of privacy in terms of differentially private basis and use technqiues such as Federated learning and Secure Multi party computation for privacy preserving deep learning classification.
  
       
     
