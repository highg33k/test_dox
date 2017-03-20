# Doximity data analyst technical challenge
#### _Proprietary and Confidential_


## Problem outline
Consider a scenario where you work for a social network company for academics. This social network includes full professors, assistant professors, postdoctoral students, graduate students and others as members. To increase engagement and interaction among the members of this academic community, your product manager wants to roll out a feature that ranks members in the network according to the number of times other people have viewed their social profiles. The product manager sketches out a general vision for the product, which would appear differently for each user:

__________

Your rank for profile views

1. John Doe
2. Jane Doe
3. You
4. Jon Doe
5. Jan Doe
6. ...

__________


Working as the data team’s point person on this project, you are responsible for pulling together and manipulating relevant data to advise the product manager on how the data can drive this new feature forward. Central to these tasks are the tables in your company’s database that contain user information and profile view records. To help you familiarize yourself with where the data live, here's a view of the schema:


![image](https://cloud.githubusercontent.com/assets/11825080/24101830/05da96b6-0d37-11e7-90b7-5926e103dd46.png)


## Explanation of DB tables

**1. users:** table containing information about the members of the academic network   
**2. user_titles:** table containing job titles; foreign key in users is title_id (magenta)   
**3. user_profile_urls:** tabulates user_id and its associated profile url used internally   
**4. internal_profile_views:** tabulates all profile views that occurred within the social network application; logged as user_id who views the profile of viewed_user_id  
**5. external_profile_views:** tabulates summary information about clicks on public_profile_urls that occur off of search engine searches  

## Connecting to the DB
The following instructions are for installing a MySQL application to help you connect to our interview database (options are contingent on your OS, and while we propose the two applications below, you can feel free to use alternative methods of your choosing): 

**1. Using SequelPro (if using a mac OS) http://www.sequelpro.com/download**

Once downloaded and installed, you can connect to our database by opening a connection window and providing the following details for a "Standard" connection:

- Host: 54.86.230.73
- user: candidate
- password: Doximity
- Port: 3316

**2. Using MySQL Workbench http://dev.mysql.com/downloads/workbench/**

Similarly, opening a connection window and providing the above information.

__________

## Part I

The product manager has some questions on the data and is looking to you for some insight. Please provide your answer (and any applicable SQL queries you used to arrive at the answer):

1. What is the average age of users by region?
2. Could you provide a breakdown of user title and number of user counts associated with each title?
3. Who is the top viewed user, based on internal profile views?
4. Can you provide a ranked list of the top 10 most view users based on internal profile views, supplemented with data from the user table? 
5. Which region gets the most viewed users (based on internal profile views)?

__________

## Part II

With these data, your goals are:
- To understand and help the product manager understand how users are interacting with each others’ profiles
- To understand how much web traffic user profiles are receiving and from where
- To pull the data in a form that can generate a “Rank for profile views” feature
- To postulate how the data may best be presented in this product.

To this end, you should create (1) one or two data visualizations to help the product manager understand the social network’s profile views data and (2) write a brief summary communicating how the data may be used to drive the product forward.

This problem is very open-ended, so feel free to investigate questions of your own that may help address the needs of the product/product manager. Below are two guideline questions that you may use for starters:

1. What is the most interesting insight or opportunity that you discovered?
2. What possible improvements to the data would you like to make?

__________

## What to submit 
**When time is up, please submit all the code you wrote, your data visualizations, answers to the questions and written summary in a pull request. We hope this exercise is helpful (maybe even fun!) for you and appreciate your taking the time to do it!** 

------------

## How to use github to submit the assignment in a pull request

* **DO NOT PUSH TO MASTER**, **DO NOT FORK THE REPOSITORY**
* Clone this repository, create a local git branch and commit your changes to said branch.
* Push branch to GitHub.
* Once work is completed, create a new Pull Request between master and your branch.
* *Upon completion, notify Dean Lucas & Alex Schearer via email (dlucas@doximity.com, ashearer@doximity.com).*
