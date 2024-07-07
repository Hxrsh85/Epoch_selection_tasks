# Epoch tasks

**Epoch task 1**\n
This task consisted of visualizing the dataset and catching some insights.
1) Data cleaning: I had first extracted my state pincodes and then preprocessed them
2) filling missing: I used mean of division's lat long values to fill in the missing lat long
3) Making a box: I made a box around Karnata and removed any values that lied outside it
4) Correcting the human error: a lot of values of latitudes had very close longitutdes, so I removed them
5) clustering: I used K-means to cluster my datapoint. The cluesters of my dataset when K = 30 resembeled very closely the district map of karnataka, hence the distribution of the post office is like the distribution of the districts
I used ploty to create interactive maps

**Epoch task 2**\
The task had three parts 
1) Aphabet recognition: I made a cnn model to recognise my 28*28 alphabet
2) image segmentation: Very early on I was able to decipher that the target image is made by stiching a lot of 28*28 alphabets. So my task was to break the images into it's constituents and pass it on to the cnn model to predict the alphabets and put it in a string which would then be passed on to my lstm model for sentiment analysis.
3) Sentiment analysis: I used a stacked Lstm model to predict the sentiment of the sentences, since the dataset was too small the efficency of this deep learning model could be achived at it's max, however I had passed the string into it and got a predictoin of the sentiment.

I also used a naive bayes classifer, which turned out better as compared to a deep learning model. However I had used Sklearn to impliment it. I've written few bits of code for the self code of naive bayes and I'm confident that I'd have completed it had I had more time.\

Kindly go throught both the notebooks, I've made texts where ever necessary for you to have better readability of the code.\
To load a particular model (cnn model = asli_model, lstm model = lstm_model) just download the models provided in github and load them with appropriate paths.

