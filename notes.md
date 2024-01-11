# my notes for the machine learning project

## steps to the project

### 1. form a hypothesis
a hypothesis is a statement we can either prove or disprove 
using data.

<b>hypothesis:</b>
we can predict how many medals a country will win in the 
Olympics

### 2. find the data
i will use data from the summer olympics.
each row is a country in a single olympics.

### 3. reshape the data
once data is acquired, data needs to be reshaped to make 
machine learning possible.

the medals will be predicted, and the athletes and 
previous medals columns will be used to make the 
prediction. the data is basically already how it needs to be.

### 4. clean the data
make sure the data is ready for machine learning.

a lot of data contains missing values. in this case, 
for some teams, there will be no previous medals, perhaps because they did not compete in that particular olympics.
a lot of machine learning algorithms cannot work when there
are missing values.

### 5. error metric
find an error metric that we can use to evaluate the 
performance of the machine learning model.

the machine learning model will create predictions. those 
predictions will be different from the actual count.
we need to use an error metric to determine if the predictions
are good or not. the error metric that will be used is 
mean absolute error. we will subtract the predictions from the 
actual values and take the mean of the actual errors.

### 6. split the data
we want to split the data because we want to train on one part
of the data and predict on another part of the data. the 
reason we want to do that is because if we train the algorithm
on the same data that we use to evaluate it, it's like the 
algorithm having an open book on the test. if it does good on 
the test, it could be because it memorized all the answers or 
had all the answers, not necessarily because it understood all
the material. we want to give the algorithm a new set of data
that it hasn't been trained on. the new set of data will 
tell us how well the algorithm is performing.

### 7. train a model
we will use linear regression, a very popular machine learning
model.

linear regression uses an equation. we will use an equation that
allows us to use two predictors: 
Y = a<sub>1</sub>x<sub>1</sub> + a<sub>2</sub>x<sub>2</sub> + B
