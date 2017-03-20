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


Working as the data team’s point person on this project, you are responsible for pulling together and manipulating relevant data to advise the product manager on how the data can drive this new feature forward. Central to these tasks are the tables in your company’s database that contain user information and profile view records. To help you familiarize yourself with where the data live, see a visual of the table schema on the next page.



Briefly,
users: table containing information about the members of the academic network
user_titles: table containing job titles; foreign key in users is title_id (magenta)
user_profile_urls: tabulates user_id and its associated profile url used internally
internal_profile_views: tabulates all profile views that occurred within the social network application; logged as user_id who views the profile of viewed_user_id
external_profile_views: tabulates summary information about clicks on public_profile_urls that occur off of search engine searches

__________

## Part I

The product manager has some questions on the data and is looking to you for some insight. Please provide your answer (and any applicable SQL queries you used to arrive at the answer):

What is the average age of users by region?
Could you provide a breakdown of user title and number of user counts associated with each title?
Who is the top viewed user, based on internal profile views?
Can you provide a ranked list of the top 10 most view users based on internal profile views, supplemented with data from the user table? 
Which region gets the most viewed users (based on internal profile views) ?

__________

## Part II

With these data, your goals are to understand and help the product manager understand how users are interacting with each others’ profiles, to understand how much web traffic user profiles are receiving and from where, to pull the data in a form that can generate a “Rank for profile views” feature, and to postulate how the data may best be presented in this product.

To this end, you should create one or two data visualizations to help the product manager understand the social network’s profile views data and write a brief summary communicating how the data may be used to drive the product forward.
__________

This problem is very open-ended, so feel free to investigate questions of your own that may help address the needs of the product/product manager. Below are two guideline questions that you may use for starters:

What is the most interesting insight or opportunity that you discovered?
What possible improvements to the data would you like to make?

** When time is up, please email us all the code you wrote, your data visualizations, answers to the questions and written summary. We hope this exercise is helpful (maybe even fun!) for you and appreciate your taking the time to do it! ** 


------------

## Assignment Instructions

* **DO NOT PUSH TO MASTER**, **DO NOT FORK THE REPOSITORY**
* Clone this repository, create a local git branch and commit your changes to said branch.
* Push branch to GitHub.
* Once work is completed, create a new Pull Request between master and your branch.
* *Upon completion, notify Dean Lucas & Pat Blachly via email (dlucas@doximity.com, pblachly@doximity.com).*
