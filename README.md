# Making AlexNet CNN inefficient using NiaPy's evolutionary algorithms
Predicting images from  ILSVRC dataset using AlexNet. Then recreating the correctly classified image(s) using NiaPy's evolutionary algorithms, trying to recreate it as similiar to original as possible, to the point, that AlexNet fails its prediction.

## Requirements
* Python 3.6+
* Pip
* NiaPy 2.0.0rc12 (pip install NiaPy==2.0.0rc12 ; included in AlexNetDiplomska.ipynb) 

### Warning
Code is in early stage, some paths etc. are still hardcoded. Images used for CNN are on my GoogleDrive, therefore there can be a problem accessing them. 

### Current plan
Transforming "bejzbol.jpeg" to same shape as array "iskanje", running NiaPy over it and displaying newly created picture. 
Using cv2 hopefully [SOLVED] Battling with a bug, that does not display image from array, if array has been modified whatsoever.
Currently working on only one picture 

![Baseball](./bejzbol.JPEG?raw=true) 
