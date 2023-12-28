# Social Buzz Social Media Analysis
This is a part of a portfolio project from [The Foarage](https://www.theforage.com/) designed by [Accenture](https://www.accenture.com/us-en). All individuals mentioned except for [Derik Vo](https://www.linkedin.com/in/derik-vo/) are fictitious.

The purpose of this project is for me, a teacher and mentor, to review the project and determine how effective this would be in evaluating student data skills. Although this project only uses Excel, students may have the opton to in additional to Excel use SQL, Tableau, or Python. I will primirly be using Python during my review, but students will not be required to use it. Essentially I will be evaluating how effective this would be as a capstone project for my students.
# Background

Social Buzz is a fictitious social media company that emphasizes user anonymous user interactions. The primary interaction between users is reacting to shared media. Social Buzz tracks type of media,type of category, and type of reaction. The company has over 500 million active users who post over 100 thousand pieces of content every day.


# Problem statement

Social Buzz aims to IPO by the end of next year, and needs to scale their processes prior for a successful launch. They aim to initiate a 3 month pilot project to audit their data practices, identify recommendations for IPO success, and identify categories with the highest user engagement.

# The Team
|Role|Name|
|------|--------|
|Data Analyst| [Derik Vo](https://www.linkedin.com/in/derik-vo/)|
|Chief Technology Architect|Andrew Fleming|
|Senior Principal|Marcus Rompton|
|Data Scientist|Michelle Grove|

# The Data

Below is the provided datasets along with the associated data dictionary

### Content

|Column|Data Points| Dtype | Description |
|------|--------|---------|--------------|
|Content ID|1000|object| Primary key for content table|
|User ID|1000|object|Foreign key for user table|
|Type|1000|object|The type of media (photo, video, gif, or audio) |
|Category|1000|object|How the content is categorized (Food, animals, technology, etc.)|
|URL|801|object|URL to the content|
### Reactions

|Column|Data Points| Dtype | Description |
|------|--------|---------|--------------|
|Content ID|25553|object|Foreign key for content table|
|User ID|25534|object|Foreign key for user table|
|Type|24573|object|The type of reaction (disgust, dislike, scared, etc.)|
|Datetime|25553|object|The timestamp of when the reaction occurred (YYYY-mm-dd hh:mm:ss)|

### ReactionTypes

|Column|Data Points| Dtype | Description |
|------|--------|---------|--------------|
|Type|16|object|Primary key for the reactiontypes table|
|Sentiment|16|object|Indicates if a reaction is positive or negative|
|Score|16|object| The numeric value of the reaction (appears to range from 0 to 75) |
