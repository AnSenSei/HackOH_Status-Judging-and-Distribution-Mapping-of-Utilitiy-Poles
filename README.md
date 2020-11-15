# HackOH Status Judging and Distribution Mapping of Utility Poles
![test](https://github.com/favicon.ico) Liangyu Liu, Junhao Qi.  

This is the project accomplished in HackOHI/O 2020 and is for competing in the challenge of AEP challenge.  
using open soucre gis api:arcgis to accomplish mapping and interactions. poping up informations such as latitude  longtitude, working status and object imagines. 

![image](https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/DistributionMapping.png)  


(The repo is to be uploaded and completed by judging time in the 2nd day of HackOHI/O.)    



This Jupyter Notebook is for requesting AEP pole detection API. The Post send contains images and get bounding box information as return. Then the notebook uses returned info to crop the image to pop utility poles out for status prediction.   


     
<img width="200" height="1000" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/PoleDetectionSample.PNG"/>        

 



         
         
Dataset       

<img width="800" height="600" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/Dataset.png"/>     

Model    

<img width="600" height="800" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/ModelSummary.png"/>      
<img width=600" height="600" src="https://github.com/LiangyuLiu/HackOH_Status-Judging-and-Distribution-Mapping-of-Utilitiy-Poles/blob/main/Deliverables/Accuracy%20and%20Loss.png"/> 


Refernece:
   

Simonyan, K., & Zisserman, A. (2014). Very deep convolutional networks for large-scale image recognition. arXiv preprint arXiv:1409.1556.  


Build an app to interactively select and display an ArcGIS Online basemap https://developers.arcgis.com/labs/javascript/select-a-basemap/     
