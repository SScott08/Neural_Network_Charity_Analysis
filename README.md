# Neural_Network_Charity_Analysis
Overview:

The purpose of this project was to create a machine learning neural network to create a binary classifier that is capable of predicting if applicants will be funded by Alphabet Soup.  I used a csv file that contained over 34,000 organizations that Alphabet Soup has funded previously. The dataset contains metadata about each organization such as:

•	 EIN and NAME—Identification columns

•	APPLICATION_TYPE—Alphabet Soup application type

•	AFFILIATION—Affiliated sector of industry

•	CLASSIFICATION—Government organization classification

•	USE_CASE—Use case for funding

•	ORGANIZATION—Organization type

•	STATUS—Active status

•	INCOME_AMT—Income classification

•	SPECIAL_CONSIDERATIONS—Special consideration for application

•	ASK_AMT—Funding amount requested.

•	IS_SUCCESSFUL—Was the money used effectively

Data Processing, Compiling, Training of the model

The csv data is read into a DataFrame and then cleaned for processing

•	Drop the EIN and NAME identifier columns

•	Convert STATUS and ASK_AMT to str ('object') type

•	Bucket the categorical variables if needed. In this case, CLASSIFICATION, APPLICATION_TYPE and ASK_AMT

•	Encode categorical variables using one-hot encoding

•	Merge one-hot encoded features and drop their original columns

•	Prepare for processing by splitting into training and testing datasets

•	Scale the data so it can be processed

•	Run several models to attempt acquiring a 75% accuracy score


Summary:

After several attempts and not achieving a higher accuracy by adjusting the neurons, adding a hidden layer, with activations of “sigmoid” instead of “relu”, my model was underperforming at ranges from 73%-74%. I went back to the columns I had removed and added more data back I put the NAME column in and re-ran the model with 100 epochs. The model began performing at an accuracy of 95%-96% which is well above the desired range of 75%.  In summary, additional data solved the problem because their was mor information to draw from. 
