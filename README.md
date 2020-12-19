# COMS-6998-Final-Project
Columbia University COMS 6998 Practical Deep Learning System Performance Final Project and Report.  Exploring the Time Series to Image Approach  


In these notebooks we take financial indicators and turn them into images which are used the train a convolutional neural network.  The images are labeled buy, hold or sell and the network looks a the 15 day trailing indicators and predicts which action to take.  Three versions are tested, a baseline, a model with additional features and a model using Inception blocks.  First run the Time Series To Image for Equites notebook and then take the CSV files it outputs and run them in the Analysis notebook to see how well the models do.  You will need a Quandl key to download the equities data, if you don't have you it shouldn't be hard to get the same information from Yahoo Finance but you will have to make some changes to get the Open, Close, High, Low and Volume into the dataframe.  

For training and testing we use 28 equities of the DOW-30.  To run tests on different equities, enter their ticker symbol into the list of equites.  Make sure that the dataframe has data going back 15 trading days from the start of your training and test periods or it will not have data to build the image. 

The paper we wrote for the project is also in the repository if you are curious about the choice we made or want to understand how the models work.

We would like to thank Professor Parijat Dube for teaching the course and providing us with valuable feedback on the project.  We would also like to thank Google for providing GCP credits for students.
