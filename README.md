# Evaluating MLP and Logistic Regression on XOR Dataset

## Impact of Feature Engineering and Regularization


### MLP

The MLP model gave a higher accuracy over the test data. $L_1$ and $L_2$ regularizations prevent overfitting in neural networks and improve the accuracy of predictions over the test data.

We can see that here the train data was generated in a particular range and so it did not have much outliers.

So, while training the MLP without regularisation also does not incur overfitting. This is the reason why the accuracies of MLP with and without $L_1$ and $L_2$ regularizations are all high and close. Since the amount of noise or outliers in the train data were very less.

The accuracy of classification increased for both $L_1$ and $L_2$ regularizations after varying the penalty coefficient by choosing the best one using a validation dataset.


### Logistic Regression

When only $x_1$ and $x_2$ are used as features the accuracy is low and the decision boundary is a straight line. It does not perform well since XOR Dataset is not linearly separable.

When $x_1$, $x_2$, $x_1^2$, $x_2^2$ are used as features the decision boundary is some curve but the accuracy and per class precision are still low.

When we use $x_1$, $x_2$, $x_1*x_2$, $x_1^2$ features we get a near to perfect classification with a very high accuracy and precision. This happens beacuse after including the feature $x_1*x_2$ the xor dataset becomes linearly separable in a higher dimensional space.