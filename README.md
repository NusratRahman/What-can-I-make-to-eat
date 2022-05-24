# WHAT CAN I MAKE TO EAT
## Table of Contents:
[Description](#description)  |  [Recipe API](#-recipe-api)  |  [Email API](#-email-api)  |  [Technologies Used](#-technologies-used)  |  [Team Members](#-Team-Members)

## Description
People are often looking for ideas of what to make to eat. Users can log into this application and provide a list of ingredients they have on hand to receive recipe suggestions based on those ingredients. They can view full recipe details and choose to have recipes they like emailed to them. In addition, users can sign up to receive a daily email that contains one recipe that matches preferences they provide.

## Recipe API
Recipe application - main point of direct interaction with user
- User sign-up/sign-in/sign-out
- In the moment recipes : User provides food items on hand, makes requests to 3rd party API for recipes using those items, user can select a recipe from ideas provided to get full details in one or more of the following ways:
  - Display in Web Browser
  - Email API sends the recipe to user by email
- Daily Recipes: User can sign-up for a daily recipe email which will be based on criteria they provide (e.g., vegetarian, vegan, dessert etc.) and the criteria is updated in the database, otherwise they will get a popular recipe everyday
- User can unsubscribe from receiving daily email anytime and all the data related to his subscription will be deleted from database

## Email API
Email application will work in the background to
- Send “In the moment” recipes that the user requested in Recipe API
- Send email daily with recipe (ideally tailored email based on user's preferences, if there is no preferences then one popular “recipe of the day” will be sent)
- Check for users that have opted into daily email (listed in database) and send email automatically
- Check that the user doesn’t receive the same recipe within the last 30 days by referencing database

## Technologies Used
- Java - version 1.8 
- Spring Boot – version 2.6.7
- MySQL Workbench – version 8.0 
- JUnit - version 5.8.2
- Docker – version 20.10.14 
- Git - version 2.35.1.windows.2 
- Kubernetes
- Jenkins
- Prometheus
- Grafana
- Spring Mail 
- Rapid API : Spoonacular API (Recipe - Food - Nutrition)

## Team Members
- Aneesh Chulliparambil Mohanan
- Anju Naduthuruthel Kumaran
- Daryl Nauman
- Nusrat Rahman
