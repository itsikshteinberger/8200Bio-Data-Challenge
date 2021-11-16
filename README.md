# 8200Bio Data Challenge
<br/>
<p align="center">
<img src="https://images.newscientist.com/wp-content/uploads/2019/05/03155847/gettyimages-932737574-2.jpg" alt="drawing" width="800"/>
</p><br/>
In this challenge the goal was to predict the medical specialty from the transcription field,<br/>
that is for each file (unique transcription) need to predict whether it belongs to each label (medical specialty).<br/>

You can find the data [here](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Data/data.csv).
And the full code [here](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Solution.ipynb).

## My strategy

* __Word2Vec:__ Convert text to vector of strings not including classification and words meaningless in term of classification.
<br/><br/>
* __StringVec2FloatVec:__ Convert Vector Numbers The vector numbers are used using one of the common conversion methods.<br/><br/>
* __Dealing with unbalanced data:__ The data is not balanced! We will duplicate the underrepresented data so that the classification is balanced.<br/><br/>
* __Train & Test models:__ Training different classic models for best results.<br/><br/>

## And what actually happened :sweat_smile:
I converted the texts to vectors using two ways (after cleaning of the data of course):
* By frequency.
<br/>

* TF-IDF Score.
<br/>
<img src="https://miro.medium.com/max/1200/1*V9ac4hLVyms79jl65Ym_Bw.jpeg" alt="drawing" width="450"/><br/>

Since in the test result the second method brought a better result I stayed only with it. <br/><br/>

Then since the data is unbalanced I tried to balance it in two methods:
* Over-sample.
* Smote.

The Smote did not work really well for this data so I gave it up.
<br/><br/>
__Now it's time for training!__  <br/>

For each specialty I trained 9 different models and chose the best of them. <br/>

The models were:  | 
------------- | 
Naive Bayes  | 
Logistic Regression  | 
K-Nearest Neighbours |
Support Vector Machine |
Decision Tree |
Bagging Decision Tree |
Boosting Decision Tree |
Random Forest |
Voting Classifier |

Except for one specialty, we had great scores.

![](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Data/image1.png)
> Example

![](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Data/image2.png)
> Final results
<br/>

## Crush the accuracy with deep learning!
Since no model returned good results to surgery specialty I decided to build a simple deep learning model for it from 2 fully connected layers. <br/>
![](https://github.com/itsikshteinberger/8200Bio-Data-Challenge/blob/master/Data/image3.png)
> Loss curve

<br/> After 30 epochs I got a nice result of 86% - maybe I will play with the network in the future to improve the result.
When we tested the models on new data we got a nice result of 93%.

<br/>

__So we can say that pretty good models have been created.__

