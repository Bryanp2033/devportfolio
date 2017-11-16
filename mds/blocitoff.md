---
layout: post
title: Blocitoff
thumbnail-path: "img/bloccitoff_mockup.png"
short-description: A self-destructing to-do list application.

---

{:.center}
![]({{ site.baseurl }}/img/blocitoff_nrmal_img.png)

<a href="https://github.com/Bryanp2033/Blocitoff">Source Code</a>
{: style="color:gray; font-size: 110%; text-align: center;"}

## Summary

There lot of modern “To-do lists” applications on the market either free or paid, for Blocitoff I wanted to challenge myself and built one myself that provides a simple experience for the users without the hassle of multiple unnecessary components. Blocitoff also takes the hassle off multiple reload pages with the integration of ajax into the project.

This project took around a week of development and was finished sometime around Jan 2016.

## Explanation


The application allows users to create a to-list where items can be marked off as completed or self-destruct/delete the item after a 7 day window.

## Challenges

Some issues I came across during production was properly intergrating a user authentication system as I felt that for an application like this with personal information being a major factor, security was a major priority. Another issue is properly styling and making a proper format on how I wanted the to-list to be presented. I wanted to style it in a way that looked neat, and modern with integrating icons for a more user-friendly experience. As well, I faced with the task of making the process of the to-list faster for the user, for a web application where making an item and saving it to the database, I face the challenge of how I could i make the process faster then it already was.

## Solutions

The solutions for user authentication was not creating the feature from scratch but rather focus on implementing a gem that allowed me the opportunity to intergrate even more factors into the user authorization process. In the end I worked with Devise, a gem and a flexible authentication solution I needed for the project. I incorporated it and configured most things from the pre-made package of the gem to my liking. This way the mailers were working as I intended for email confirmation and reseting password, as well creating the relationships needed for the user and their items.

For styling I needed a faster solution and I ended up working with Bootstrap, a front-end framework provided by Twitter, this allowed me to work with pre-made front-end styling while configuring and creating new ones on my own. This is exactly what I ended up doing during the stages of presenting the list itself. I ended up working with a table html tag and incorporating some bootstrap styling within the tags. The end result was the table showing list of items, on each row included the item name, how many days the item will be there before getting considered "expired", and a checkpoint glyphicon provided by Bootstrap to mark off the item/task as completed.

As for implementing a faster system for the to-do list process, I came to the conclusion that a solution would be to get rid of page reload of a POST request when creating the item, for this I intergraded ajax , a client-side script that communicates to and from the database without the need for page refresh. With this, the process of the app took less longer then expected and since I also incorporated ajax for the deletion feature for the item, the outcome was also a faster process as I intended it be, thus creating a better user-friendly app without the hassle of waiting for items to load in/delete.

## Conclusion

Overall for my project I'm glad for what I achieve and any further improvements towards the project I can see doing are minimal.