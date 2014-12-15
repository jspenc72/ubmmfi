# Purpose of the Application

  - The Application will Store a standard set of objects, their attributes and behaviors of those objects that exist in the UBM Master File Index.

# User Inferface Components
Users will interact with the system through the following components. 
  - A mobile app which the user will load on their iPhone or Android device. (see End- User Interaction)
  - A web interface for uploading the target images.

# Language Preferences
> One of our goals is to simplify crossplatform
maintenance and distribution. To that end, we prefer mobile apps which are developed in HTML5 / CSS3 / JavaScript. However, we will entertain proposals for
alternative solutions or native languages. Please email us at ubmoffice9@gmail.com to discuss
alternatives.

#Server Environment
- Webbased components should be able to run on a standard LAMP stack using shared hosting.

# End-User Interaction

> The primary user interaction will be via a mobile application distributed via the Google Play and Apple App

##### Mockups

>Need to create them on pixt.io or draw them by hand.

##### Basic workflow (Mobile)
  - The User will load the page (app)
  - The User will sign into the application
  - The User will be shown a dashboard with a graph that displays the number of each ubm object that they have created.
  - The User will swipe left to see a menu with each type of ubm object that they may create.
  - When one of the objects in the list is selected the user is presented with an interface that may use a compination of popups and a dynamic list of the selected object type to perform CRUD operations on the application.
  - 

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma start
```
