#Travel Assistant Web App

This is a machine learning project that implements regression and recommendation system techniques to provide travel recommendations for users. 
The project is built using Python and deployed as a web application.

#Requirements

Python 3.x

Scikit-learn

Pandas

Numpy

Streamlit

Ngrok

Animations used in the web app is done using Lottie files


#Stage 1 : Collection of Data and Processing

Data for this project is collected from Kaggle.

Data is directly accessed from Kaggle and processed for the further usage.

This process involves the aggrigation of 14 - lakhs datapoints to 15,000 data points . Aggregated based on the unique places in the data around India.

Reviews from the data is processed, compressed and made into hashtags with the use of Word cloud module.

You can find the this process as a seperate .ipynb file named Clarity TTS Data Preperation


#Stage 2 : Recomendation Engine building 

Here the processed data from stage 1'st utilized.

A recommendation engine is developed using the cosine similarity consept.

This will recommend you some similar placed as like your favourite place by getting your favourite placce or intrested place as input.


#Stage 3: Regression Model - Flight Ticket Price prediction

Data source for this model is Kaggle.

This data consist of 6 different location avation history data with 3 lakh data points.

A Regression model is built using Random Forest Regressor, XGB Regressor and Linear Regression and XGB is finalized for the deployment with the R2 score of 95 % and MAE of 2188.435237364721


#Stage 4 : Web App Building.

This web app is built using Streamlit library and Ngrok is used to tunnel the web server into the localhost as this app is built in Google Colab.

This Web app is named as "Your Travel Assistant" consist of 3 parts.

##Home Page Interface
![image](https://user-images.githubusercontent.com/119114780/234227589-1dc47935-9ac7-4e97-b86c-e1caf19ae2ee.png)



##Part 1 : Flight Ticket price predictor

Here Inputs like Boarding point, Destination, Prefered boarding time, prefered arrival time, Class, Prefered Airline, No of Stops and Days before booked were feeded to predict the price of the flight ticket using the pickled XGB model.

##Predictor Interface
![image](https://user-images.githubusercontent.com/119114780/234227711-e9806096-8536-4c17-a0f7-f4d0661ac446.png)



##Part 2 : Tour Place Recomennder

Here inputs like Intrested / Favourite place, State, and no of places want were feeded and some recommendations were displayed whick were similar to the your intrest.

##Recomender Interface
![image](https://user-images.githubusercontent.com/119114780/234227787-251a402f-4a39-42f0-99ea-5591b4b97b5f.png)

![image](https://user-images.githubusercontent.com/119114780/234227807-08f545be-97e9-46f0-97fb-961835399289.png)



##Part 3 : Tour Place Explorer

This is the place where you can drill down by state and city to view the available touist spotss in that place. 
This is dome using chunking down the data by State and city wise as per the user input


##Explorer Interface
![image](https://user-images.githubusercontent.com/119114780/234227908-51fc29dd-9406-4451-b0da-016f403acc51.png)


#Future Improvements

Expand the dataset to include more destinations and activities

Improve the recommendation system by incorporating user feedback and ratings

Implement natural language processing to improve user input and search results

Add more features such as weather information, transportation options, and travel tips
