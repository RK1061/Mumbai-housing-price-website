This project demonstrates the development of a machine learning model to predict house prices in Mumbai based on features like the number of bedrooms, bathrooms, area, and stories. The model is built using Python, Scikit-learn, and Pandas, and the trained model is serialized using pickle for deployment or further use.
Features
Linear Regression Model: Used to predict house prices.
Input Features:
bedrooms: Number of bedrooms.
bathrooms: Number of bathrooms.
area: Total area of the house in square feet.
stories: Number of stories in the house.
Target Variable:
price: The price of the house.

Dataset
The dataset (housing.csv) includes the following columns:
bedrooms
bathrooms
area
stories
price

step for setup
If you don't have virtualenv installed, you can install it via pip
pip install virtualenv
virtualenv env
After creating the environment, you need to activate it
.\env\Scripts\activate.
after that install
flask - pip install flask
pip install pandas scikit-learn
Place the housing.csv dataset in the root folder of your project.
Run the following script to train the model and save it to model.pkl: - python train_model.py
To make predictions with the trained model,  use the following code in your Python scrip : import pickle
model = pickle.load(open('model.pkl', 'rb'))
new_data = [[3, 2, 1500, 2]]
predicted_price = model.predict(new_data)
print(f"Predicted Price: {predicted_price}")
 File Structure
 housing.csv          # Dataset file
 train_model.py       # Script to train the model
 model.pkl            # Saved machine learning model
 requirements.txt     # Python dependencies
 README.md            # Project documentation
Requirements
Python 
Pandas
Scikit-learn






