# Restaurant Guest Mobile Application
## Overview
This Android application is part of the full ['Restaurant Guest Software System'](https://github.com/users/RonnieLutaro/projects/5). The System makes use of a Mobile Application and a Real-time Analytics Admin Dashboard. Both the Admin Dashboard and Mobile application consume a RESTful [Web API service](https://github.com/RonnieLutaro/restaurant-guest-REST-API). The vision here is to develop a more efficient way for restaurants to manage their business operations and Customer Experience while receiving and accepting digital payments from their customers.

## Inspiration 💡
Small businesses in Uganda are faced with customer management challenges that lead to business failure as stated in a [research](https://www.researchgate.net/publication/291863118_Causes_of_small_business_failure_in_Uganda_A_case_study_from_Bushenyi_and_Mbarara_towns) that was carried out by Kazooba, in 2006.
Research was conducted on 133 small business enterprises including **restaurants**, bars, hotels, and others, it turns out that most of the small businesses in Uganda fail due to a number of factors that result from management problems, inadequate control of inventory, delays in processing applications among others (Kazooba, 2006). The Idea to develop an innovative solution that solves the challenge of small Restaurant business failure gave birth to the 'Restaurant Guest Software System'. 

## Technologies used 🚀
* [Java SE](https://www.oracle.com/java/technologies/javase-downloads.html) 
* [Android Studio](https://developer.android.com/studio)
* [Firebase](https://firebase.google.com/)

## Setting Up 🛠

1. `git clone https://github.com/RonnieLutaro/restaurant-guest-android` to any desired directory location on your computer.
2. In order to start configuring, you need to install [Android studio](https://developer.android.com/studio/index.html) >= v3.0 and the [Java SE Development Kit](https://www.oracle.com/java/technologies/javase-downloads.html) before continuing to the next step. 
3. To import, simply open Android Studio and use **Open an Existing Project** action, navigate to the directory where you cloned this repo and select it to import. Be sure to wait for all the processes (the Gradle Build) to complete before continuing to the next step. Accept licenses to download **SDK 28** if prompted to do so. Alternatively, you may navigate to the **SDK Manager** within Android Studio and manually install **SDK 28**. If you get a popup that prompts you to sync gradle click on OK, then wait until the import is done.
4. Create a [Firebase](https://firebase.google.com/) account.
5. Now navigate to your firebase console, create a new project with the same package name as the project's so you can enable the push noification API.
6. If everything went well, firebase will generate a **google-service.json** file, download it and save it on your computer.
7. Inside your android studio, navigate to **google-service.json** and replace it with the new one, now sync your project.
8. Return to the firebase console to get the firebase key, settings > Cloud messaging > copy your server key and paste it in your dashboard field.

**Note :**
Please don't update your gradle version to the latest version , this may cause a lot of issues after this transaction. After compiling the source code in android studio you will be faced with the following message "Failed to resolve: play-services-auth", it's caused by the google-services.json that should be generated on firebase console and placed on the android project folder
