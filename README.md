# Convolutional Approach to Sentiment Classification

Machine  learning tasks can usually be categorized into two main groups, classification and regression. Classification describes the more straight forward approach of determiningthe class of a certain input. These classifications can be verysimple binary classification of for  example cats and dogs or more complex multi-class classification with multiple possible categories. Regression differs from classification in the way that the end goal usually represents any real value and is not limited to acertain number of classes. Regression usually revolves around predictions, for example stock predictions or sales predictions.

## Data Set overview
The dataset used is the Rotten Tomatoes movie review sentiment dataset. The dataset consists of reviews with their associated sentiment. There are a total of 5 sentiment classes, 0-4. The dataset is very imbalanced as class 2 has significantly more samples than the other calsses.

### Final Model

The final model consists of only three convolution layers where the first two were followed by a max-pooling layer as well as a dropout layer with a dropout of 0.25. The third convolutional layer did not have a pooling or dropout layer. The kernel sizes in the first two layers had a kernel size of five while the last one had a kernel size of 3. A total of three dense layers are used in the final model, the first layer contains 256 neurons and is followed by a dropout layer with a dropout of 0.25. The second layer had 128 neurons and was followed by a dropout with a factor of 0.5. The last layer contained 5 neurons to perform the prediction on the one-hot encoded label.



## Test Results
The results can be view in the report pdf.


## Authors

* **Tim Heydrich** - *Initial work* - [legerdemainist](https://github.com/legerdemainist)

See also the list of [contributors](https://github.com/Legerdemainist/NLPAssignment2/graphs/contributors) who participated in this project.


## References
A. Fisher and P. Sikka, “Lab 4: Multilayer 1d conv classification networkin pytorch."
cacoderquan, “Sentiment-analysis-on-the-rotten-tomatoes-movie-review-dataset,”https://github.com/cacoderquan/Sentiment-Analysis-on-the-Rotten-Tomatoes-movie-review-dataset/blob/master/tra
