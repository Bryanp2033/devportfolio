---
layout: post
title: Bloccit
thumbnail-path: "img/bloccit_mockup.png"
short-description: A application allowing users to create, delete and share topics, posts, and comments.

---

{:.center}
![]({{ site.baseurl }}/img/bloccit_nrmal_img.png)

<a href="https://github.com/Bryanp2033/Bloccit/tree/user_profile">Source Code</a>
{: style="color:gray; font-size: 110%; text-align: center;"}


## Summary

Nowadays there a lot of forum types sites like Digg, Reddit, etc. devoted to providing content like news, stories, gifs, pictures all centered around different types of topics to subtopics devoted to that specific type of community.

This project is an inspiration of what I was trying to achieve, it was my first coding project ever and it centered around creating a site where users can create topics and creates posts to those said topics.

It wasn't an original idea, but merely a project to test my skills in web development, none the less this project is still a fully fletched out one with various amounts of features, from liking and favoriting posts, to making user profiles the option to incorporating a user profile picture, to creating comments.

This project took 1 month in development and finished sometime around October 2015.

## Explanation

It was the first project to teach me the fundamentals of web development all in the while doing most of this on my own with sometimes additional help and yet still making the end result of the project into a fully functional one.

The application allows users to create a topics, post, comment on posts without a page reload(ajax requests), favorite the posts, check out their own and other users' profiles' displaying the topics and posts they created, diverse user features allowing them to display a user profile image. They can also check out the most current favorite posts and popular users, and the app also displays the list of topics and posts with pagination.

## Problems

Some of the problems I face during the development process was implementing a proper relationship system between topics, posts, and comments. I had the task of applying CRUD features to all of these while maintaining hierarchy system where users can create topics but can't create the comment without creating the post. Another issue was finding a solution in integrating a more diverse option for users to distinguish themselves from just their username.

## Solutions

The first solution I found for this was simply configuring the code and nesting the post resources/routes under the topic resources all in the while creating the topic_controller into a folder where the post_controller was also nested under it.

This was to insure complete control of the topic and relationship it had with the post that way it was confirmed and tested that a post could only be created if ONLY the topic for it existed. This was a similar solution for the comments feature and as well intergrating a dependent destroy method within their models, that also had assurance that if a comment were to be deleted by the user, the post that contained it would not be deleted.

For the second solution I found the best option for distinguishing users was to implement a uniqueness validation via the devise gem in the user_model that way a username that was created would always come out to be different.

As well I implemented a image uploading feature for user profiles using a little help of the carrier_wave(for uploading the images) and mini_magick(for proper image re-sizing) gems. This feature was the best solution I found to be as it provided the user the opportunity to use a image(with guidelines attached to it)and make their account a bit different from the rest.

## Conclusion

For this and how the features came out to be, I'm proud of this project and how it turned out. In the near feature what future improvements I could see myself doing is find unforeseen problems where DRY code could be a solution.