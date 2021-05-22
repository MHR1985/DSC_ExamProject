# DSC_ExamProject
## Authors:
Martin Høigaard Cupello, Kenneth Leo Hansen, Frederik Blem, Simon Bojesen

# Stage 1:
## Idea 1 : Kidney disease prediction
### Focus of interest:
To detect possibility of chronic kidney disease given certain parameters.
### Why is it interesting:
It will  help to discover the sickness early and therefore enable treatment at an early stage. Or in preventative medicine.
### Which outcome do you expect from your research:
To create a model which will be able to a high degree of success to predict if a person is sick with chronic kidney disease.
### Who will the user be:
A docter or other medical staff.

## Idea 2 : Fake news detection
### Focus of interest:
There is a huge amount of fake news articles on the internet. This will help discover them, so they can be avoided.
### Why is it interesting:
It is interesting because it will enable you to only get "true" news to a certain degree.
### Which outcome do you expect from your research:
A model which can be used when for example scraping the internet for articles and collect "true" news.
### Who will the user be:
Facebook, twitter and so on.

## Idea 3 : Closed eyes facial recognition for sleepy drivers alert
### Focus of interest:
To prevent drivers from falling asleep while driving.
### Why is it interesting:
It will prevent some accidents from occuring.
### Which outcome do you expect from your research:
An ai which can determine if the person in the image/video has his eyes closed, and then play an alert if that is the case.
### Who will the user be:
Occupational truck drivers for example.

# Stage 2

## 1. All of the relevant  datasets are stored in the Data folder.

## 2. ELT/ETL and part 3 Data processing scenario 

##  Kidney disease prediction
[Notebook](Python/kidneyNotebook.ipynb)
<br/>
#### Datastory:
With the data we have gathered we will try to find out which columns is a factor when detecting chronic kidney disease. With the data we have visualised we can see that hemoglobin is a very important factor when diagnosing ckd. We can also see that the older you get the higher chance of being diagnosed with chronic kidney disease.
![Dashboard](Images/dashboard/dashboard_kidney.png)

##  Fake News Detection

[Notebook](Python/NewsPrediction.ipynb)

### Dashboard
![dashboard](Images/dashboard/news_dashboard.jpg)
#### Datastory
The idea is to find word occurrences in the articles, and from these, determine if an article is true or fake news.

In the figure on the right we can see that most articles with the subject "politicsNews" or "worldnews" fall in the category of true news, where the mean for the other subjects are fake news. It does not mean that fake news cannot have a subject of politicsNews for example, just that the average does not.

The word occurrence figures show how many times a given word appears in the text/title. There is a lot of similarities found here for common words, but there is a few that stands out, for example in the word occurrence for fake news title, the word "Video" and "Watch" appears in this toplist, where it does not appear in the true news.

## Closed eyes facial recognition for sleepy drivers alert

# Stage 3
We choose to go with the chronic kidney disease project. The AI is created in the notebook.

## AI Module
To create the AI Module we have split the data into 70% training data and 30% test data.
By testing different machine learning algorithms, we created a model that provides 98,28% accuracy when diagnosing a patient with chronic kidney disease or not.
In our tests the inaccuracy resulted only finding false negatives with an error rate of 3% when determining if a person has chronic kidney disease. Also during our tests there were no false positives, which means it has a 100% accuracy when determining if a patient does not have chronic kidne disease. 

# Stage 4
We have created our HeatMap in VR with color and size coding of the different features, depending on the impact on the classification. Here is the link to the video, click view raw to download:
[video](Images/virtualReality/DSC_VRSpheres.mp4)

![img](Images/virtualReality/vr.png)

<b><em>Elaborate on the benefits of applying better visualisation techniques for data analytics:</em></b>

It increases the engagement and understanding of the target audience, rather then showing raw data, enabling them, who has no prior knowledge of data science, to make decisions.

One important aspect of better visualisation is that it enables better overview of corrolation between the features in the data. It also helps with the understanding of the data that the model is based on.

One of the benefits of visualisation is to see trends over time, providing a basis to be able to make predictions. In order to make predictions you need to be able to see what has happened in the past and present, enabling you to predict the future.







