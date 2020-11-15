# HackOH Status Judging and Distribution Mapping of Utility Poles
![test](https://github.com/favicon.ico) Liangyu Liu, Junhao Qi.  

This is the project accomplished in HackOHI/O 2020 and is for competing in the challenge of AEP challenge.  
using open soucre gis api:arcgis to accomplish mapping and interactions. poping up informations such as latitude  longtitude, working status and object imagines. 

![image](https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/DistributionMapping.png)  


(The repo is to be uploaded and completed by judging time in the 2nd day of HackOHI/O.)    


First we have a Jupyter Notebook used for requesting AEP pole detection API. The Post send contains images as body and get bounding box (pole position) information as return. Then the notebook uses returned info to crop the image to pop utility poles out. This notebook is also used for data cleaning in building a training dataset and pole working status judge in neural network predicting.    


     
<div align=center><img width="100" height="500" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/PoleDetectionSample.PNG"/></div>        

 



         
         
Dataset       

<div align=center><img width="600" height="450" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/Dataset.png"/></div>    
The data set contains around 750 images of utility poles, and divided to traing set and testing set at a ratio of 0.8/0.2. Each image has a label which can either be {'disposed': 0,'in-service': 1,'in-maintenance': 2}       



Model    

The trainig method we used in this project is transfer learning(Using VGG16 as base model  pretraind with imageNet). The reason we choose is that it can suit the situation of having a small dataset and 
easily adapt to future complicated tasks (over a simple neural network).         



<img width="600" height="800" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/ModelSummary.png"/>      
<img width=600" height="600" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/Accuracy%20and%20Loss.png"/> 

	
 Performance:      
 

The model we built can achieved an accuracy of 93.9% on testing set.   


Distribution Mapping:        

Using open source api Arcgis to create the map to show the distribution using points shows a pop up when clicking on the point containing information of geographic information, working status object imgines       







Refernece:
   

Simonyan, K., & Zisserman, A. (2014). Very deep convolutional networks for large-scale image recognition. arXiv preprint arXiv:1409.1556.  


Build an app to interactively select and display an ArcGIS Online basemap https://developers.arcgis.com/labs/javascript/select-a-basemap/     
