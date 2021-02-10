# Making AlexNet CNN inefficient using NiaPy's evolutionary algorithms
Predicting images from  ILSVRC dataset using AlexNet. Then recreating the correctly classified image(s) using NiaPy's evolutionary algorithms, trying to recreate it as similiar to original as possible, but only to the point, that AlexNet fails its prediction.

## Requirements
* Python 3.6+
* Pip
* NiaPy 2.0.0rc12 (pip install NiaPy==2.0.0rc12 ; included in AlexNetDiplomska.ipynb) 

### Warning
Code is in early stage, some paths etc. are still hardcoded. Images used for CNN are on my GoogleDrive, therefore there can be a problem accessing them. 
#### 2 versions
Because of that, there are currently 2 versions of Jupyter Notebook. 
* "AlexNetDiplomskaColab.ipynb" that requires Colab, my gDrive etc.
* "AlexNetDiplomskaLocal.ipynb" that runs 2 pictures and NiaPy locally

### Current plan
* a) Evaluate the difference between original and recreated picture - something similiar to RMSE - average difference in pixel - bigger differences (errors) get bigger punishment
* ?) Should NiaPy change only targeted parts of the picture - used in CNN prediction? 
* [DONE] Transforming "bejzbol.jpeg" to same shape as array "iskanje", running NiaPy over it and displaying newly created picture. 
* [SOLVED] Using cv2. Found bug, that does not display image from array, if array has been modified whatsoever.


![Baseball](./bejzbol.JPEG?raw=true)
![Tiger](./tiger.jpg?raw=true) 
