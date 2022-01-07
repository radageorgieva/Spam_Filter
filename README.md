# SPAM FILTER

This is part of a group assignment I completed during the Machine Learning module of my MSc studies. The underlying dataset consists of SMS data from the UCI Machine Learning Repository. The main goal of this assignment is to build a Naive Baye's Spam Filter.

## Installation 
### Downloading the Data
- Dowload the Spam Filter.ipybn notebook and open in virtual environment
- Download the data files from https://archive.ics.uci.edu/ml/machine-learning-databases/00228/

    
### Installing the requirements
- The python version is Python 3.8
- You're better off using virtual environment 
- Find all required packages and their corresponding version in the file requirements.txt

## Full Article 

## Conclusions of the project

The aim of this paper was to determine whether representation biases exists in machine
learning for medicine, why they exists, and how they can be reduced. To do so, it
leveraged current literature and an empirical study consisting of the prediction of acute
liver failure with a focus on the potential differences in its performance for the two
genders.

Literature suggests that representation bias is present in algorithms, as it is in
the judgment of people. On one hand, this final paper confirms the existence of such
disparities in machine learning for medicine through an exemplary case, in which there
is a significant bias with an ambiguous source and a surprising direction. On the other
hand, it also proves that the enhancement of such prejudice by machines is preventable,
as the inequality in performance for different social groups can be mitigated with the
help of technological tools.

The solution offered is the one of giving a weight to each data point based on their
demographic characteristic of interest and their dependent variable value. The weights
should be given according to the fairness and optimization criterion, which, in the case
of medicine, is sensitivity. It is important to note that, differently by common beliefs,
it is not the most underrepresented group that should necessarily be given highest
importance but rather the discriminated one. In the study, this group is the one of
sick men. The weights given to data points according to their dependent variable value
can be determined by the type of values optimized by the chosen score. In sensitivity
this is the true positives; thus, patients with acute liver failure should be given more
importance. This method manages to not only mitigate the bias but also improves the
overall sensitivity.

Unfortunately, these results are achieved at the cost of the reduction of other
performance metrics such as accuracy. The chosen solution is the one that harms this
score the least but also manages to mitigate the discrimination. The rest of the proposed
solutions have sensitivity close to 100% but it does not mean that they perform well.
For example, one can also get trivially to 100% sensitivity when classifying everything
as positive but the resulting model would not be reliable. The final solution has an
overall sensitivity of 91.1%, a 1.7% bias benefiting women and reduces accuracy by
5.3%(much less than the other proposed solutions).

Because of the limitations of this study it might be best if a hybrid approach is
used in the deployment of this technology. According to it, there should be a balance
between algorithm and human judgment. The ways to develop it depend on the different
applications of the models. If embraced by a Private Clinique, the models could be
used only to determine whether further examinations should be done to confirm the
diagnosis rather than whether a treatment should be started. Moreover, physicians
should be trained to work side-by-side with the algorithm to achieve optimal use of the
technology.

Instead, if the algorithm is deployed on an app, it might be best to be transparent
with the users about the performance of the model. They should be aware that, while
there is a low probability that they are told to be healthy, but are actually not, there
still is a significant possibility that they are told to be sick, but are actually healthy.
Hence, the algorithm shall be used as a mechanism to suggest visiting a doctor or
scheduling further examinations.

