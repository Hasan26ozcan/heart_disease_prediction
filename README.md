# heart_disease_prediction
I tried heart disease prediction with sigmoid and SVM models, and I found that the SVM model was more successful.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/ccf948b9-5b23-4eda-9d2a-0921e6f4fce9)


I'm using SVM and the sigmoid function in my neural network, and the SVM model is working quite well. Firstly, I check the code for missing values, and it looks good because there are no missing values in the data. Next, I examine the data, and although there are no missing values, there may be outliers. I found outliers in the cholesterol and old peak values. You can see visual representations of these outliers.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/e7d9950b-2767-4b71-a986-60cc73c23e51) ![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/2c807e03-ba71-419e-acfe-d69ce6b0ed8c)

First, if you need to fill in some '0' values in your data, I started thinking that these values might indicate missing information. So, I decided to keep these '0' values as placeholders to represent unknown information.

Then, I thought about creating a model to predict the missing values. As a first step, I trained this model using 'training data (x_train)' that included all data except for the 'cholesterol' value. Then, I used this model to make predictions for the missing values and placed these predictions in the places marked as '0'. This way, I obtained a more consistent dataset.

Now, I'm ready to start writing the prediction model.

Firstly, I created a sigmoid prediction model

here is my sigmoid function prediction rate:

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/6239fc5a-79fd-4351-922a-7a834c1a116f)


I'm using an SGM model for prediction. 
First, I need to find the best kernels, and I'm using this code block to do so.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/8785ce28-230f-4598-ac35-bad11844ad23)


I see that the polynomial and RBF graphs perform the best. However, I'm thinking about how I can find the best graph kernels. If I check the other data values on the kernels, I can find it. If you want to take a look at these graphs, you can see them in code.


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/c7622ee6-c792-4a49-8805-8313b4c2cb64)


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/d285f22f-81cf-49d3-97c8-0b1880006f37)


I've discovered that polynomial kernels work best, so I'm using polynomial kernels for the prediction.

Before I start the evaluation, I need to create the graph for the prediction model.


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/71b02bfe-7579-4932-aa62-4f974372a2a4)


This is my prediction model. I can see the best gamma values are 0.035 and 0.065. While the prediction of 0.065 is not bad, the prediction of 0.035 is outstanding. My best gamma value is 0.035, and I want to use a confusion matrix because I want to see all the predictions in one list. If you want to see it in a graph, you can open the code block. Actually, a list is sufficient for me.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/7936c9fe-5541-4852-9899-a537b44eab4a)

Actually, my code block contains a value of 0.065. If you want to see the 0.065 value, you may need to change the print function in the code we wrote.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/0d5df397-848d-43b1-bb5f-001a2f4a2d9f)



