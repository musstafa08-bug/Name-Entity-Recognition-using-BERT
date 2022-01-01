# Name-Entity-Recognition-using-BERT


## PROBLEM STAEMENT
In this project we will be prforming one of the most famous task in the field of nautal language processing i,e Name Entity Recognition.
DESCRIPTION OVERVIEW
Named EntitiesRecognition (NER) is a basic task of Natural Language Processing (NLP). The purpose is to identify named entities such as person names, place names, and organization names in the corpus. Due to the increasing number of these named entities, it is usually impossible to exhaustively list them in the dictionary, and their constituent methods have some regularities. Therefore, the recognition of these words is usually included in the task of morphological processing (such as Chinese segmentation). Independent processing, called named entity recognition. 

Named entity recognition technology is an indispensable part of many natural language processing technologies such as information extraction, information retrieval, machine translation, and question answering systems.

Named entities are the research subjects for named entity recognition. Generally, named entities include 3 categories (entity, time, and number) and 7 categories (person, place, institution, time, date, currency, and percentage). Judging whether a named entity is correctly identified includes two aspects: whether the boundary of the entity is correct; and whether the type of the entity is correctly labeled. 

The main types of errors include correct text, which may be of the wrong type; conversely, text boundaries are incorrect, and the main entity words and part-of-speech tokens it contains may be correct.


## TECHNOLOGY USE
Here we will be using  Anaconda Python 3.6 , Pytorch 1.4 with GPU support CUDA 10 with CuDNN 10.



## INSTALLATION
 Installation of this project is pretty easy. Please do follow the following steps to create a virtual environment and then install the necessary packages in the following environment.

### In Pycharm it’s easy 

1. Create a new project.
2. Navigate to the directory of the project
3. Select the option to create a new new virtual environment using conda with python3.6
4. Finally create the project using used resources.
5. After the project has been created, install the necessary packages from requirements.txt file using the command pip install -r requirements.txt


### In Conda also it’s easy

1. Create a new virtual environment using the command
    conda create -n your_env_name python=3.6
2. Navigate to the project directory.
3. Install the necessary packages from requirements.txt file using the command         
pip install -r requirements.txt

## Workflow Diagram
![workflow_dig](https://user-images.githubusercontent.com/64519071/147853172-27428bba-5187-46f8-baa7-664bc9c12b56.jpg)

## IMPLEMENTATION
### 1. Project Directory
![project_directory](https://user-images.githubusercontent.com/64519071/147853181-12d37727-d6a2-4236-a2e2-c22f85394236.png)

This above picture shows the folder structure of the project. Here data folder consists of data and out_base folder consists of the BERT models.

### 2. requirements.txt	
![requirements](https://user-images.githubusercontent.com/64519071/147853183-42a43875-45f4-4b04-af68-811da631c780.png)

requirements.txt file consists of all the packages that we need to run with project.

### 3. bert.py
![bertpy](https://user-images.githubusercontent.com/64519071/147853189-ce039efc-b57d-4d47-8904-165c4fa20e6f.png)

This is the most important file in this project which we will be using for training and prediction.


### 4. clientApp.py
![clientApp](https://user-images.githubusercontent.com/64519071/147853190-90356e67-189e-4578-a260-8a2fa7559245.png)
This is the flask server file and the entry point of application.


## TESTING IN LOCAL/API
To do the test testing we need to run the clientApp.py and after that web server will start at http://0.0.0.0:5000/


Enter the Text and click on Predict button.
![bert](https://user-images.githubusercontent.com/64519071/147853228-dec90ab0-988b-4095-9384-ca56f66e6a8a.png)

Predictions will be shown in the result box. 
![Results](https://user-images.githubusercontent.com/64519071/147853230-92a88455-dc01-4854-ae60-4d9e49e6db79.png)
