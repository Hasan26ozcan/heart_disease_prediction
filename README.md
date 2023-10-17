# heart_disease_prediction
I tried heart disease prediction with sigmoid and SVM models, and I found that the SVM model was more successful.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/ccf948b9-5b23-4eda-9d2a-0921e6f4fce9)


I'm using SVM and the sigmoid function in my neural network, and the SVM model is working quite well. Firstly, I check the code for missing values, and it looks good because there are no missing values in the data. Next, I examine the data, and although there are no missing values, there may be outliers. I found outliers in the cholesterol and old peak values. You can see visual representations of these outliers.

![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/e7d9950b-2767-4b71-a986-60cc73c23e51) ![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/2c807e03-ba71-419e-acfe-d69ce6b0ed8c)

First, if you need to fill in some '0' values in your data, I started thinking that these values might indicate missing information. So, I decided to keep these '0' values as placeholders to represent unknown information.

Then, I thought about creating a model to predict the missing values. As a first step, I trained this model using 'training data (x_train)' that included all data except for the 'cholesterol' value. Then, I used this model to make predictions for the missing values and placed these predictions in the places marked as '0'. This way, I obtained a more consistent dataset.

Now, I'm ready to start writing the prediction model.

















firstly ı made a sigmoid predict model
and its my sigmoid fuction predict :


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/6239fc5a-79fd-4351-922a-7a834c1a116f)



and ı make a sgm model predict:

first ı have to find best kernels and ı'm using this code block


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/8785ce28-230f-4598-ac35-bad11844ad23)


and ı see the poly and rbf graphs are the best 
but ı have to find best graphs kernels and ı2m thinking how can ı, and if ı check the other data value on the kernels ı can find it
if you want to look this graphs you can see that


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/c7622ee6-c792-4a49-8805-8313b4c2cb64)


![a](https://github.com/Hasan26ozcan/heart_disease_prediction/assets/91744709/d285f22f-81cf-49d3-97c8-0b1880006f37)


and ı found the poly kernels is the best and ı'm using the poly for the predict kernels 

and the time for the evaluation first ı must the graphs for the predict model







