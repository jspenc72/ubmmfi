#UBM Master File Index System
The latest version of this documentation and specification may be found here:

> http://ubmmfi.readthedocs.org/en/latest/Specification/

Edit project documentation here:

> https://github.com/jspenc72/ubmmfi/


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

# Administrator Interaction
  - The primary administrator interaction will be to review objects that have been created by users and request the user to publish the object to make it available to all users or a specific user.
  - Initial seeding of template objects will likely be accomlished by copying and pasteing existing objects from online or other sources. (Any method of automating this seeding step would be greatly appreciated.)

##### Basic Workflow

Administrators will need the following functions:
  - Object Management
    - Single and Bulk import of template objects.
    - Single and Bulk creation of template objects.
    - Single and Bulk view of template objects.
    - Single and Bulk update of template objects.
    - Single and Bulk deletion of template objects.
  - User Management
    - Ban a User for any reason
      - Should retain users email and prevent them from logging in.
  - Method for exporting database to .csv format for excel import and manipulation.

# Online / Offline Interaction
  - The mobile application should be able to run entirely offline.
  - The mobile application does not need to include every possible template object for offline access.
    - The application should cache ~10 most popular objects of each type.
  - A user’s documents created offline should be synchronized with to the server periodically.

# Data Entities
The following are the core objects and their attributes or essential methods. 

##### Legal Entity
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - models []

##### Model
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - positions []

##### Position
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - jobs []

##### Job
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - policies []

##### Policy
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - procedures []

##### Procedure
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - steps []

##### Step
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
  - tasks []

##### Task
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
 
##### Product
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

# Suggested Relational Model
##### Legal Entity
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Model
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Position
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Job
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Policy
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Procedure
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Step
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Task
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  
 
##### Product
  - title
  - description
  - createdBy
  - createdAt
  - updatedAt  

##### Instance
  - instancetype
  - instanceid
  - createdBy
  - createdAt
  - updatedAt  

##### Instance Closure Tree 
  - id
  - ancestor_id
  - descendant_id
  - path_length
  - createdAt
  - updatedAt

# Exported CSV File Schema
Administrators will need to export a csv file for each object in the database, or for a set of objects that are of the same type. They should have to option to export all objects created by a single user. Or any Subtree of the UBM Heirarchy.

# Delivery Method
The following deliverables are required:
  - A .zip compressed archive with the appropriate files:
    - source code for mobile app (Android and iOS, if developed separately)
    - source code for Administrator Interface
    - .sql file or migration file which may be used to generate the web-based databases via phpMyAdmin or through some other command line interface.
    - Instructions with steps for implementation
    - Github Repository with source code.
    - readthedocs.org project documentation.

# Planned Features
Although not inteded as features for this release, potential feature for future releases include:
  - Enabling Users to log in via Facebook and Google accounts
  - File attachements (jpg, gif, pdf, docx, xls) to all objects.

# Additional Questions / Deviations From This Specification
Please submit questions to ubmoffice9@gmail.com with the subject line "UBM MFI SYSTEM RFP"

This specification is intended as a starting point for dicsussion and our attempt as answering some common development questions. Deviations from the spec are acceptable as long as they are approved by us before work takes place and documented as a change order once the project has been awarded.



```sh
$ 
```
