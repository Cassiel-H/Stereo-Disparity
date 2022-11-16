
# University of Melbourne COMP90086 Computer Vision project - Stereo Matching

School of Computing and Information Systems

1. [Introduction](Introduction)
2. [Requirements] (Requirements)
3. [Main Components](Main Components)
4. [Major Results](Major Results)



## Team Members

* Haonan Lyu - halyu1@student.unimelb.edu.au - 1252105
* Jiachen Huo - jihuo@student.unimelb.edu.au - 1293736

# Introduction 

The purpose of this project is to develop a complete and necessary stereo matching pipeline, with multiple matching techniques( inclusing baseline model), result discussion and error analysis.

"Stereo matching is the problem of finding correspondences between two images that are taken simultaneously from two cameras that are mounted so that they are parallel and separated along their x-axis. The output of stereo matching is a disparity image that, for every pixel in the left image (x), indicates how many pixels to the left its correspondence (x’) is in the right image, giving the disparity (x-x’)." [Source here](https://github.com/Cassiel-H/Stereo-Matching/blob/main/Stereo%20Disparity%20project.pdf)

![IMAGE ALT TEXT HERE](https://github.com/Cassiel-H/Stereo-Matching/blob/main/img/project_disparity.png)

In this repo, we had the following major working pipelines:
1. Image preprocess (i.e. adding border effect). 
2. Implement multiple window-based matching technique/functions (e.g. SSD, ZSSD and ZNCC)  
3. Develop optimization strategies (e.g. smoothing, Gaussian Kernel, strided matrix calculation, enabling GPU .etc) 
4. Examine matching accuracy with different:  
  - Window Size;  
  - Matching Functions 
5. Error Analysis


# Requirements
- To run CV_proj.ipynb, place it in the same directory of the Dataset folder. 
- A CUDA Toolkit is required to run CV_proj.ipynb
- Python version and other libiary requirements as in requirements.txt 
```python
pip install -r requirements.txt
```

# Main Components
CV_proj.ipynb has two main section
1. Design Step: contain functions about the baseline SSD model and optimized models
2. Evaluation Step: contain results of each model defined in Design step

# Major Results

