# Making AlexNet CNN inefficient using NiaPy's evolutionary algorithms
Predicting images from  ILSVRC dataset using AlexNet. Then recreating the correctly classified image(s) using NiaPy's evolutionary algorithms, trying to recreate it as similiar to original as possible, but only to the point, that AlexNet fails its prediction.

## Requirements
* Python 3.6+
* Jupyter Notebook environment
* Pip
* NiaPy 2.0.0rc12

#### 3 versions
Code is in early stage, some paths etc. are still hardcoded. Images used for CNN are on my GoogleDrive, therefore there can be a problem accessing them. Because of that, there are currently 3 versions of Jupyter Notebook:
* "NiaPyDiplomskaLocal.ipynb" that uses 2 pictures and NiaPy locally - specified in [requirements.txt](requirements.txt)
* "AlexNetDiplomskaColab.ipynb" that requires Colab, my gDrive etc.
* "NiaPyDiplomska.ipynb" that uses 1 picture (tiger.jpg), NiaPy and CNN prediction in Google Colab. *Important! Download files!*

### Current plan
* a) Evaluate the difference between original and recreated picture - something similiar to RMSE - average difference in pixel - bigger differences (errors) get bigger punishment
* ?) Should NiaPy change whole or only targeted parts of the picture - used in CNN prediction? 
![CNN Layers - Visualization of the activation maps](https://miro.medium.com/max/785/1*mzmytBNCTO3CEKtpCVxIRA.png)


![Tiger](./Images/tiger.jpg?raw=true) 

## Looks promising
Original: ![Baseball](./Images/bejzbol.JPEG?raw=true)
After NiaPy: ![BaseballMissed](./Images/zanimivost.jpg?raw=true) 
