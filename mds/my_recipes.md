---
layout: post
title: MyRecipes
thumbnail-path: "img/myrecipes_mockup.png"
short-description: A web application where users can create and share recipes and review them.

---

{:.center}
![]({{ site.baseurl }}/img/myRecipes_nrmal_img.png)

<a href="https://github.com/Bryanp2033/myRecipes/tree/review_feature">Source Code</a>
{: style="color:gray; font-size: 110%; text-align: center;"}

## Summary

In the IOS market and Google Play store, I noticed there was lot of recipe finding and recipe making apps, as for this project this was my twist of the idea behind those types of applications. This was a project for me that had familiar ground to it as some of these features were the same of Bloccit(one of my other projects) but with different and new features and custom-made ones like the user authentication feature but from scratch. This project took a month in development and was finished sometime around June 2016.

## Explanation

This project idea was not original as before me there were already similar apps out there either for displaying use or deploying it to the app store. For me this was a just a passion project as a beginner chef lately, I wanted to provide a application for users to create and share recipes all in while other users can review it.

The application allows users to create a recipe with/without a picture, post,reviews without a page reload(ajax request), like the recipes, check out their own and other users' profiles showcasing their recipes, and the app also displays the list of topics and posts with pagination.

Lastly, users can create new ingredients and recipes styles to effectively distinguish what type the recipe is and what ingredient it as as that was priority for me as a safety concern(allergy reasons, etc.) for the users.

## Problems

The problems I came across towards development was finding a solution or an idea to create a feature in which users can effectively look for what type of recipe they looking for. I was looking at the big picture as my thought was if there would be multiple entires of recipes in the database how can one distinguish the differences of the recipes?.

Another problem I came across was how I wanted to tie the relationship between the user and the recipe and how I would present it. That way other users can check out the recipes of other users as a way to look at their other works.

## Solutions

For the first solution was to create a feature where users can create ingredients and recipes styles and thus giving them the opportunity to tied them into their recipes all in the while it automatically creates an index of recipes containing that ingredient it contains or recipe style it is. For example now instead of two banana puddings recipes in the database, it can now be differentiated by the types of ingredients it contains or recipe style it is, if it's either Greek or Italian and thus making two entries different despite the same name. The ingredient feature was also a success for me as it solve a problem I had previously foreseen and that was establishing more safety precautions for users for specific food allergies.

For the second problem, the solution I found was creating an index on the users#show view page displaying all of those user's recipes that way it's establishes a showcase of all the user's work and creates a reputation for themselves.

## Conclusion

For this project and how the features came out to be, I could see some further improvements and features like integrating a favorite user feature to principally follow/heart the user as their favorite chef. As well I could see myself making more improvements to the ingredients and recipes styles page by creating uniqueness validations to them and make limit space on how many entires can be added to the database, as the big picture I see if too many entires in the database for even the page to load or the user to frustratedly navigate too. As of now for displaying a simple task for a small user-base this application gets the work done just fine.