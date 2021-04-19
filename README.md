# Restaurant Guest Mobile Application
This Android application is part of the full ['Restaurant Guest Software System'](https://github.com/users/RonnieLutaro/projects/5), a name that was originally given to this system as part of the naming process for a project title. Traditionally, this kind of system would be referred to as a Restaurant Operations Management System.

## Inspiration
Small businesses in Uganda are faced with customer management challenges that lead to business failure as stated in a [research](https://www.researchgate.net/publication/291863118_Causes_of_small_business_failure_in_Uganda_A_case_study_from_Bushenyi_and_Mbarara_towns) that was carried out by Kazooba, in 2006.
Research was conducted on 133 small business enterprises including **restaurants**, bars, hotels, and others, it turns out that most of the small businesses in Uganda fail due to a number of factors that result from management problems, inadequate control of inventory, delays in processing applications among others (Kazooba, 2006). The Idea to develop an innovative solution that solves the challenge of small Restaurant business failure gave birth to the 'Restaurant Guest Software System'. 

This System makes use of a Mobile Application and a Real-time Analytics [Dashboard](https://github.com/RonnieLutaro/restaurant-guest-dashboard). Both the Dashboard and Mobile application consume a [Web API service](https://github.com/RonnieLutaro/restaurant-guest-dashboard). My intention with this project is to develop a more efficient way for restaurants to manage their business process and customer experience. 

## Impact of the solution
According to a survey carried out by ZDNet, 5.7 hours is the average time spent by millennials on phones each day, while baby boomers devote 5 hours to smartphone use. However 13% of millennial and 5% of boomers say that they spend over 12 hours every day on their phones. 

With all this information put into consideration, a software solution that capitalized on mobile smartphone usage was accounted for as the best canditate.
This solution will enable customers to be able to access their favorite restaurant's available menu items, place their oders and have them processed through the mobile application. Customers can either decide to takeaway or have their order home delivered.

## How to set up
### Install Android studio
In order to start configuring , you need to install Android studio and the 'Java SE Development Kit'.
Make sure that you have installed the latest version of android studio 3.+, if not please download it from this [Link](https://developer.android.com/studio/index.html)
### Import Android Project

1. To import, simply open Android Studio and use the (Get from Version Control) action, provide the repository url and make sure to wait for all the processes (the Gradle Build) to complete before continuing to the next step.
2. If you get a popup that prompts you to sync gradle click on OK , then wait until the import is done
3. Now navigate to your firebase console ,create a new project with the same package name so you can enable the push noification api
4. If everything went well, firebase will generate a google-service.json file, download it and put it in your computer
5. Open your android studio , then go to google-service.json and change it with the new one , now sync your project
6. Return to the firebase console to get the firebase key , settings > Cloud messaging > copy your server key and past it in your dashboard field

**Note :**
Please don't update your gradle version to the latest version , this may cause a lot of issues after this transaction. After compiling the source code in android studio you will be faced with the following message "Failed to resolve: play-services-auth", it's caused by the google-services.json that should be generated on firebase console and placed on the android project folder
