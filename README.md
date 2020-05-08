# Plagiarism Detection Model

Plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text.

Deployed on AWS SageMaker.

[see the list of notebooks](https://github.com/blawok/plagiarism_detection/search?l=jupyter-notebook)

[**Feature Engineering**](https://github.com/blawok/plagiarism_detection/blob/master/2_Plagiarism_Feature_Engineering.ipynb)

[**Training and Deployment of the Model in SageMaker**](https://github.com/blawok/plagiarism_detection/blob/master/3_Training_a_Model.ipynb)

Random Forest model on three features that I have created:
* Intersection of the 1-gram word count (containment)
* Intersection of the 9-gram word count (containment)
* Longest Common Subsequence

Model achieves 96% accuracy - one observation was missclassified (red dot). 
![plag](https://user-images.githubusercontent.com/41793223/81398954-7d982b80-912a-11ea-972c-dacec4ad7fd0.JPG)

In further research I will try out simpler, linear models, they may have perform better on this dataset. 

Anyway, for an ultimate plagiarism detector I will implement transformer based model on text data.
