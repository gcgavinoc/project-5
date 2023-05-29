# Gaming News Site
Welcome! My name is Gavin O'Connor and this is . In this project, the goal was to create a live site that allows users to create posts based on Characters from the popular video game Overwatch 2. The characters would then be categorised and the users could set certain filters to only view characters of a certain type. User could then comment on those characters posts and upvote/downvote the comments from other users.

You can access the live site [here](https://gavin-project-5.herokuapp.com/).

![Image of site using Am I Responsive tool](assets/images/amiresponsive.png)

# Table of Contents
[User Experience (UX) Design](#user-experience-ux-design)
 - [User Goals](#user-goals)
 - [User Expectations](#user-expectations)
 - [Game Logic](#game-logic)

[Features](#features)
 - [Home page](#home-page)
 - [Post Page](#post-page)
 - [Like button](#like-button)
 - [Comment section](#comment-section)

[Testing](#testing)
 - [Manual testing](#manual-testing)

[Technologies used](#technologies-used)

[Deployment](#deployment)

[Project Screenshots](#project-screenshots)

[Acknowledgements](#acknowledgements)

# User Experience (UX) Design
[Go to top](#table-of-contents)

## User Goals
[Go to top](#table-of-contents)

The user goals for this project are the following:
 - To allow users to create posts with a title and text content as well as a header image for the post.
 - To allow users to comment on posts and to allow all users to see those comments under the post.
 - To allow users to 'like' a post to show that they agree with or appreciate the contents in the post, and to have the total number of likes appear under the post to show users at a glance which posts are favored by users over others
 - To allow users to view all posts being created for the site and to allow them to peruse the different posts for themselves to read their text content and learn about various news stories or topics of discussion.

## User Expectations
[Go to top](#table-of-contents)

The user expectations I expect when engaging with this site are the following:
 - The design should be intuitive enough for the user to be able to create a post for themselves without the need for rules screens or instructions.
 - The user should expect to be able to comment on a post.
 - The user should expect to be able to like posts.

## Site Skeleton
[Go to top](#table-of-contents)

I created a site skeleton before starting development on the site itself, which allowed me to visualize what elements and features needed to be implemented as well as to set a scope for my site that needed to be met. The site skeleton was created using [UIZard](https://uizard.io/). The site skeleton can be seen below:

![Image of the site skeleton for the home page of the site](static/images/uizard-home.png)
![Image of the site skeleton for the post page of the site](static/images/uizard-post.png)

# Features
[Go to top](#table-of-contents)

## Home page
[Go to top](#table-of-contents)

Upon loading the site, the user will be greeted with a screen that shows three buttons at the top of the screen. These three buttons will be as follows. The first is home, to return the user to the home screen where the site first loaded. The second is to create a post. The third is to login if the user has an existing account and the fourth is to register for an account.

Under that, the user will see the title of the Gaming news site. Then the posts will appear under that, with each post appearing in it's own square space, and the posts appearing on top of and next to each other in a grid formation. The posts will show the posts image as a background with the post title, author, date, and number of likes and comments overlayed onto the image. The user can click on the post they want to view to open it.

At the bottom of the screen, the user will see various links to social media sites for the gaming news site such as to Facebook, LinkedIn, and Twitter.

![Image of the home screen](static/images/home-screen.png)

## Post page
[Go to top](#table-of-contents)

When the user clicks on a post, they will be brought to the page for that post. Here they will see the title of the post, as well as the name of the author, date it was posted and the number of likes and comments. Below this there will be the image being used for the post, and below that will be the text content for the post. The comments will then appear under the text content if the user scrolls down to the bottom of the text content, as well as a box for the user to enter their own comment.

![Image of the posts page for the site](static/images/post-screen.png)

## Like button

If the user wishes, they can click on the like button associated with each post. This will increase the number on the like counter for that particular post by 1. The user can also click the like button again to 'unlike' the post, if they wish to remove their like later or if they clicked it accidentally.

![Image of the like button for the posts on the site](static/images/like-button.png)

## Comment section

Under the text content of each post will be the section for comments. There will be a text field that the user can enter their comment into and the click a submit button to have their comment appear on the post. The comments will be displayed from oldest at the top to newest at the bottom, so that other users visiting the site can see the comments in order as they were made on the post, with each comment being influenced by the ones made above it, simulating a conversation.

![Image of the comment section for the posts on the site](static/images/comment-section.png)

# Testing
[Go to top](#table-of-contents)

## Manual Testing
[Go to top](#table-of-contents)

I manually tested the site by creating posts, and then also creating comments on those posts and liking/unliking the posts as well. The post appeared correctly on the home page in a grid formation with title, author, post date and image appearing as normal. The home button also worked correctly by bringing me back to the home screen. The register button allowed me to create a new user profile and the login button allowed me to sign in as a created user succesfully. The comment field allowed me to create a post a new comment on those posts and the like button increase the like counter on each post by 1 when clicked and reduced the counter by 1 when clicked again.

# Technologies used
[Go to top](#table-of-contents)

 - [Github](https://github.com/) was used to create the repository that hosts the site and to store the project's code after it was pushed from Git.
 - [Gitpod](https://gitpod.io/workspaces) was used as the Code Editor used for the site.
 - [Heroku](https://www.heroku.com) was used to host the site code as an app.

# Deployment
[Go to top](#table-of-contents)

This project was deployed to Heroku from Github, Heroku was used to host the site as an app.

These are the deployment steps:

1. Push all code to Github
2. Go to [Heroku](https://www.heroku.com)
3. Click button labeled 'Sign up for free'
4. Enter details, click 'Create free account'
5. Click link in verification email sent to entered email address
6. Create new password, click 'Set password and Login'
7. Accept terms of service
8. Click 'Create new app'
9. Enter app name and select Europe as the region, click create app
10. Click settings tab, click 'Reveal Config Vars'
11. Enter key as PORT and value as 8000
12. Enter key as SECRET_KEY and value as chosen password
13. Enter key as HEROKU_POSTGRESQL_ORANGE_URL and value as postgres://wljjdmxfqtlxqb:8bc8d113d931b9f4f092c2153b9d418b49f6f259583e32be2b347546621786cc@ec2-54-228-32-29.eu-west-1.compute.amazonaws.com:5432/d9o84q8bicjpqu
14. Enter key as DISABLE_COLLECTSTATIC and value as 1
15. Enter key as DATABASE_URL and value as postgres://vhdjiaeu:G0NFgUewu3VsNBQnxXfjv_c7YqXXmtCh@kandula.db.elephantsql.com/vhdjiaeu
16. Enter key as CLOUDINARY_URL and value as cloudinary://274126749241213:-Cam-CM8CS3DkASjY2YAYcJzuqE@dmsbtzyq3
17. Click 'Deploy' tab, click 'Connect to Github'
18. Click 'Connect to Github', sign in to Github in window that appears
19. Search repository name in search bar 'project-4'
20. Click repository 'project-4' that appears, click 'Connect'
21. Scroll down, under 'Choose a branch to deploy' ensure 'main' is selected
22. Click 'Deploy Branch', then 'View' when deployment is complete

# Project screenshots
[Go to top](#table-of-contents)

Home page
![Image of the sites home page](static/images/home-screen.png)

Posts page
![Image of the sites posts page](static/images/post-screen.png)

# Project Issues
[Go to top](#table-of-contents)

I struggled greatly with being able to learn and comprehend Django and the intricacies of back-end development, which lead to me being unable to complete this project the way I had hoped. I have scheduled private tutoring sessions which I hope will help to bring me up to speed on this portion of the course, allowing me to return to this project and add all of the functionality I had envisioned.

# Acknowledgements
[Go to top](#table-of-contents)

 - This site is based on the code created from the Code Institute walkthrough project entitled "Moments"
 - Wireframes were created via UIZard free wireframes builder tools
 - Many thanks to my mentor Marcel for his help and guidance