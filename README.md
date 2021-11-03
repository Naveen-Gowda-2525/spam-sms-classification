# spam-sms-classification
	The business objective was to predict whether the message is a spam or a ham.
	In the first step EDA was performed to draw insights. The major insights that were drawn from the dataset was-
•	Spam messages wordcount fall in the range of 15-30 words, whereas majority of the Ham messages fall in the range of below 25 words.
• Almost 1/3 of Spam messages contain currency symbols, and currency symbols are rarely used in Ham messages.
• It is evident that most of the Spam messages contain numbers, and majority of the Ham messages donot contain numbers.
	The dataset was also checked if it was balanced or not and it was found to be imbalanced so in order to fix this over was implemented to fix it
	The data was cleaned by removing special character and numbers using regular expression, Converting the entire sms into lower case, Tokenizing the sms by words, Removing the stop words, Lemmatizing the words, Joining the lemmatized words, Building a corpus of messages.
	After performing data cleaning and  obtaining  corpus of messages a bag of model was created with the help of count vectorizer..A classification model was built by splitting the dataset into test and train dataset.
	After trying out with different classification models the naive bayes classifier was selected as the finalized model as it had a good accuracy .
	The model was deployed with flask framework and Flask API was created using heroku.

For EDA and Model Building refer - Spam SMS Classication.ipynb
For Deployment refer - app.py
Flask API link - https://spam-sms-classification-api.herokuapp.com/
