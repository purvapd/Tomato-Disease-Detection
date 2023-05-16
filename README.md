# Tomato-Disease-Detection


## Problem statement 

**The project aims to develop a deep learning model to classify tomato crops into ten categories: ['Tomato_Bacterial_spot', 'Tomato_Early_blight', 'Tomato_Late_blight', 'Tomato_Leaf_Mold', 'Tomato_Septoria_leaf_spot', 'Tomato_Spider_mites_Two_spotted_spider_mite', 'Tomato__Target_Spot', 'Tomato__Tomato_YellowLeaf__Curl_Virus', 'Tomato__Tomato_mosaic_virus', 'Tomato_healthy'] .
These are common diseases that cause significant crop yield and quality losses.**
	
Clone my Github repository on your local system :- https://github.com/purvapd/Tomato-Disease-Detection

### To create a deep learning model, follow these steps:

Step 1: Install Anaconda
https://docs.anaconda.com/anaconda/install/windows/

Step 2: Launch Jupyter Notebook

Step-3: Open the Tomato-Disease-Detection\training\training_model.ipynb notebook 

Step-4:	Run each cell

At the end of this step you will get the CNN model  version 1 in the folder 
Tomato-Disease-Detection\saved_models\1

### Create Fast API

1. Open the "Tomato-Disease-Detection\api" directory.

2. Install the necessary packages by running the command 
	
		pip install -r requirements.txt

3. Open Visual Studio Code and make sure the terminal path is set to "Tomato-Disease-Detection\api".

4. Install the uvicorn package and Run the Fast API by running the command 

		pip install uvicorn

		uvicorn main:app --reload

5. To check if the API is working or not, you can use Postman by installing it from the link provided
(https://learning.postman.com/docs/getting-started/installation-and-updates/).

6. In Postman, use the following credentials to test the API:
	
		URL: http://localhost:8000/predict

		Type: POST

		Body:

		Key: file (select file type only)

		Value: Select an image of a potato leaf as a file.

		You will receive a response as follows:

		{

		"class": "Mosaic_virus",

		"confidence": 0.9994027614593506

		}
	
###  Run website:-
1. Install nodejs 
https://nodejs.org/en/download

2. make sure the terminal path is set to "Tomato-Disease-Detection\frontend".

		Install the packages 

		pip install npm

		npm install --from-lock-json

		npm audit fix

3. Make sure FAST API is running. Now to run the website 
npm run start
	
