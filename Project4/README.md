

 <p align="center"></p>
  <p align="center" style="color:blue;font-size:35px;">Facial Emotion Recognition using EfficientNet</p>

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Acknowledgements](#acknowledgement)
6. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

if you are running in your laptop, you will need to have ananconda installed and create environment/kernel that is able to run CUDA. <br><br> 

Assuming you have installed Ananconda, you will have to create environment which is CUDA capable
    <ul>
    <li>First create the environment in conda  "conda create env --name yourenvname"
    <li>Activate that environment  "conda activate yourenvname"
    <li>conda install pytorch torchvision torchaudio cudatoolkit=11.1 -c pytorch
    Where cudatoolkit version is dependent on your gpu and test if you can access cuda with 
          Import torch
          torch,cuda.is_available()     ## the execution should return true
    <li>Install any libraries that the ipython notebook needs. Or you have other chances in the Jupyter Notebook itself
    <li>Install the ipython:  conda install -c anaconda ipykernel
    <li>Then link the environment with ipython: python -m ipykernel install --user --name=yourenvname
    <li>Finally activate Jupyter notebook and see if the environment is available within the kernel
    </ul>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. 

The code should run with no issues using Python versions 3.*. All other libraries needed is declared within the file

Or else you can upload the notebook to google colab and select GPU for your hardware accelerator type. Or better yet run in AWS Sagemaker

## Project Motivation<a name="motivation"></a>

For this project, I was creating an CNN network to solve problems of classification of facial emotion based on Kaggle Competition

      

## File Descriptions <a name="files"></a>

IPython Notebook
There are a notebook available here (Facial_emotion_recognition_v14.ipynb) to showcase work. 

Data
1) FER2013 Data is downloaded using Kaggle API. You would need to get a personal Kaggle token and stored it in .kaggle folder of your home directory (assuming you are using Ubuntu)
Alternatively, you can download from https://drive.google.com/file/d/1wFgMoc5_X15bA5j8_WRzyExsRzgyzcyh/view?usp=sharing

2) The photos use in the deployment can be found in deploy folder ie myself.png

3) Model to be used: model_c7e0_0.6620.pth file is found in the main folder

Report
Project Report and Project Proposal Report is within it

## Results<a name="results"></a>

The main result is summarised in the project report.</a>

## Acknowledgements <a name="acknowedgement"></a>

Thanks to my tutor Seng Wee and the wonderful fellow students I have for this 10 weeks

## Licensing <a name="licensing"></a>

All rights reserved

All source code and software in this repository are made available under the terms of the MIT license.



