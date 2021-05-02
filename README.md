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
