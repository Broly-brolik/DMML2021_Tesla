# Welcome on the Github repository of the Tesla Team
Formed by [Broly-brolik](https://github.com/Broly-brolik), [leyouki](https://github.com/leyouki) and [khandide](https://github.com/khandid3) , our team participates in the <img src=https://www.kaggle.com/static/images/site-logo.png width="100"> competition entitled [*Detecting the difficulty level of French texts*](https://www.kaggle.com/c/detecting-the-difficulty-level-of-french-texts/leaderboard). 


This competition is an evaluation tool for the *Data Mining & Machine Learning* course of Prof. Vlachos at the University of Lausanne.  
![unil logo](https://hecnet.unil.ch/medias/plone/lg14/logo_unil.png)  
Have a look at the: 
* [Syllabus of the course](https://hecnet.unil.ch/hec/syllabus/descriptif/2457)
* [GitHub of the course](https://github.com/michalis0/DataMining_and_MachineLearning)



You will find an actual link to our Jupityer notebook at the [code section](https://github.com/Broly-brolik/DMML2021_Tesla/tree/main/code).  
The data is accessible in the [folder of the same name](https://github.com/Broly-brolik/DMML2021_Tesla/tree/main/data).  
Some other solutions in Python language but in a different approach with other libraries can be found in the [document folder](https://github.com/Broly-brolik/DMML2021_Tesla/tree/main/documents).

We proceeded following these steps:

1) Take the training set, split it 80-20, train models on the train set and test it on the test set. But, then, when we train the model to submit on kaggle we can use all the dataset to train,

2) Calculate the baseline and all 4 precisions (of 4 models), then vary the parameters to optimize i

3) Then, use a model (or combinaison of many) after doing some data cleaning (e.g. removing stop words, lemmatization, tokenization, etc...) and compute the precision.

Finally, our best model was the logistic regression with Doc2Vec. In fact, we obtained a better socre in Kagglw when training the model only in the splitted trained set from train_data than when training in all data from train_data.

Here are the different results from the different model. The results are based on models that were trained in the train splitted data from train_data.
The baseline is 0.17

mettre tableau

Conclusion:

Our final model is quite better than the baseline. However, it could be improved using, for example, neural networks.
