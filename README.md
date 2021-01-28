# Principal-Feature-Visualization
Principal feature visualization is a visualization technique for convolutional neural networks that highlights the contrasting features in a batch of images. It produces one RGB heatmap per input image.

<img src="docs/overview_fig.png" width="480">

## About the Repo
This repo contains the following files and folders:

- **Grad Cam** folder Contains scripts for running the Grad Cam (another type of Visualization technique) along with the folders where you can put images and view results.
- **Images** folder contains all the different images used during the experiment.
- **Results** folder contains results for various kinds of objects and things along with results of different CNN models tried on Principal Feature Visualization technique. 
- **Sample Images** folder where one can put images to try PFV technique on. 
- **PFV.py** is the python script for the Principal Feature Visualization(PFV) technique.
- **Demo.py** is used to run the PFV script where you can modify different models and adjust dataset and preprocessing(if require).
- **Demo.ipynb** same as demo.py script 
- **Requirement.txt** contains all the libraries you need to run the scripts.

## Dependencies
* pytorch
* numpy

### Additional dependencies for the demo:
* torchvision
* matplotlib
* pillow

## How to use 
Make sure you have all the dependencies required to run the project(mentioned in Requirement.txt file).

Add images to the 'Sample Images' folder which you want to visualize. 

Run the example in demo.py: `python demo.py` Or  You can use the ipynb notebook to view what each line of code is doing. 
 
 **Important :** In file 'demo.py' and you can change the pretrained model weight as well by changing the line 
 ```python
model = models.vgg16(pretrained=True)
```
By default model is vgg16. If you wish to change details can be found [here](https://pytorch.org/docs/stable/torchvision/models.html) .

