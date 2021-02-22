# Making AlexNet CNN inaccurate using NiaPy's evolutionary algorithms
Predicting images from  ILSVRC dataset using AlexNet. Then recreating the correctly classified image(s) using NiaPy's evolutionary algorithms, trying to recreate it as similiar to original as possible, but only to the point, that AlexNet fails its prediction.

## Learning phase
**The algorithm recreates the whole original picture from scratch considering only the BenchMark function.** No compression or simplification of the image were used. I believe, this approach will lead us into the direction, where we can apply the procedure on **any image** of any size, that AlexNet recognizes in the first place. The future goal is to work on the AlexNet's native 224*224 resolution.

## Requirements
* Python 3.6+
* Jupyter Notebook environment
* Pip
* NiaPy 2.0.0rc12

#### 3 versions
Code is in early stage, some paths etc. are still hardcoded. Images used for CNN are on my GoogleDrive, therefore there can be a problem accessing them. Because of that, there are currently 3 versions of Jupyter Notebook:
* "NiaPyDiplomskaLocal.ipynb" that uses 2 pictures and NiaPy locally - specified in [requirements.txt](requirements.txt)
* "AlexNetDiplomskaColab.ipynb" that requires Colab, my gDrive etc. - *Full version!*
* "NiaPyDiplomska.ipynb" that uses 1 picture (tiger.jpg), NiaPy and CNN prediction in Google Colab. *Important! Download files!*

### Current plan
* How to do the same thing with NiaPy?

### Milestones
* Added **PyGan** to create a **Proof Of Concept**, proving that the idea and BenchMark works
* **Succesfully recreated** a few images. We can nicely see which pixels have been tampered with, to achieve almost **100% wrong prediction of AlexNet**
* **Added Metrics** to compare and evaluate images after recreation


![Baseball](./Images/bejzbol80-80.JPEG?raw=true) ![Nautilus](./Images/nautilus80-60.JPEG?raw=true) ![Strawberry](./Images/strawberries100-53.jpg?raw=true) 

## Looks promising
First No. represents the border, at which we, if AlexNet recognizes the actual motive of the picture, include it into the BenchMark. This forces evolutional algorithm to recreate a picture not only similiar to the original, but also in such way that **AlexNet completely fails** at its prediction
### Examples
* Recreated Baseball at 20k-32,5k: 

![BaseballRecreated](./Pygad%20Recreated/20000-32500Baseball-Bib.jpg?raw=true) 

* Recreated Nautilus with updated/fixed BenchMark at 50k-52,5k: 

![RecreatedNautilus](./Pygad%20Recreated/50000-52500Nautilus-BrainCoral.jpg?raw=true) 

* Recreated Strawberry at 20k-20,5k: 

![RecreatedStrawberry](./Pygad%20Recreated/20000-20500Strawberry-Mitten.png?raw=true) 