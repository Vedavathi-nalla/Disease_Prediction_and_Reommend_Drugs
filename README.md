# Disease_Prediction_and_Reommend_Drugs


**PROBLEM STATEMENT:**

The patient who are suffering from the disease in the beginning stage but they neglect to visit the doctor because of no time or hate visiting the hospital which can cause increase the disease into higher level. Hence it is a challenge to find out the which drug is consumed for which disease based on the symptoms and other personal details of the patients age, season, weight and so on... for diagnosing the complication that occurs due to drug interaction.
This project helps those people in such a way when they enter their symptoms, age, weight all the required inputs this project gives the disease as output by using ML algorithms. Then we used the content-based technique to recommend the drugs and specialist to meet as per the disease predicted. After taking the input we have done pre-processing to convert the input into according to the model input for testing. Then the dataset is used in the ML model building and training, then that model is used to test with the taken input to predict the disease. We use the cosine similarity matrix to recommend the drugs and specialist based on the disease predicted.


**ARCHITECTURE:**

![image](https://github.com/Vedavathi-nalla/Disease_Prediction_and_Reommend_Drugs/assets/68542087/f4de820c-b27e-4ec0-a323-e4857050fb22)


**EDA:**

Heatmap

![image](https://github.com/Vedavathi-nalla/Disease_Prediction_and_Reommend_Drugs/assets/68542087/3d573abe-a802-4c18-936b-0db26c57e8f7)



DashBoard using PowerBI

![image](https://github.com/Vedavathi-nalla/Disease_Prediction_and_Reommend_Drugs/assets/68542087/868b70c0-fcb8-4a8d-a629-1014eebd870d)



In Data Preprocessing we converted all the categorical into numerical and also converted all the strings into numbers so that we can use it to train the model. And we also splitted the dataset into train and test as 80 and 20 respectively.

We have trained the model by using 6 ML techniques that are SVC, Logistic Reg, Naïve Bayes, Decision Tree, Random Forest, XGBoost. 

For every model first we have created the model and then fitted the model with the training data then predicted the testing data by using the model then we find the accuracy of the models then we used cv as 5 and find the scores of every model. Finally, we concluded Naïve Bayes has more accuracy that is 96 percentage. Therefore, the Naive Bayes model findings were applied to recommend medicines. We applied a content-based approach for recommendations. Using disease and drug characteristics, content-based recommendation recommends medicines for similar diseases. For our content-based recommendation system, we used cosine similarity.

It calculates the cosine of the angle formed between two vectors(disease) that are projected in a multi-dimensional. The output value is between 0 and 1.
The output value is between 0 and 1. 0 denotes no similarity, while 1 denotes complete similarity between the two diseases. The recommend model recommend drugs and specialist based on high cosine similarity score for given disease symptoms.  


**Result Analysis:**

![image](https://github.com/Vedavathi-nalla/Disease_Prediction_and_Reommend_Drugs/assets/68542087/04772455-a795-4a3a-982e-6cc00f1708e0)
Based on the above picture we concluded to use RandomForest because it has 99% accuracy where as other has lesser than 80%. So to predict the disease we used Random Forest ML Algorithm.


**Test Case:**

![image](https://github.com/Vedavathi-nalla/Disease_Prediction_and_Reommend_Drugs/assets/68542087/23058c0b-cbd5-4efc-8885-62fc75bbe651)

Here by using RandomForest we predicted the disease based on the patient's input and recommended the drug and specialist.

