# Requirements

## Project Overview
We are going to prototype a basic 3 tier web application that will allow us to manage [`Swatches`](/swatches/readme.md) data easily from a browser. The **Swatches Manager** tool will provide a simple interface to view our swatches, view the details for an individual swatch, and create new swatches that will be store in our swatch database.

## Swatches Manager App Features

There are 3 general features we must support for [`swatches`](/swatches/readme.md):
- **List of Swatches** - A view that list of all of our swatches from our database. Here we can show the swatch thumbnail and the name in a list or table format. 
- **Swatch Details** - Clicking on a swatch image or name from the list view should display the swatch detail view. It shows all additional details for a swatch. Name, price, etc. Please see below for the **Swatches data model**.  
- **Add a Swatch** - A form that can be filled out to create a new swatch. The data model for a swatch can be found below. 

Users should be able to perform the below actions on the respective views/screens:
- Ability to view a list of swatches and see top level information. 
- Ability to click on a swatch from the list and view more details. 
- Ability to create a [`new swatch`](/swatches/readme.md)
- Newly created swatches should become available in list/detail views.

# Technical Spec

## Back End 
### NodeJS application requirements: 
- Develop a basic set of `CRUD` services that are exposed via an `HTTP` endpoint. 
  - Ability to `CREATE` a new a swatch
  - Ability to `READ`  swatches
  - Ability to `UPDATE`  swatches
  - Ability to `DELETE` a swatch
- The app should respond to incoming `API requests` with a `JSON` response. 
- The app should have support for `GET`, `POST`, and `PUT` methods.
- The app should query the database and return in support of incoming requests. 
- The app should update the database in support of incoming requests.
- Your NodeJS application should be deployed to an `EC2 instance`.  

##### `Note:` Please remember to provision resources using `free tier` so you do not occur any charges for this exercise. 

## Front End
### VueJS Application Requirements:
- The front end should be built using [VueJS](https://vuejs.org/). 
- Your app should leverage endpoints exposed by your NodeJS application to perform CRUD operations. 
- Your code should be easy to understand, and broken into logical. 
- Your front end build should a single page app with a single `index.html`
linking to external `JS/CSS/etc`. 

### Host It
- When Hosting your front end application, ensure it is authorized to make requests to your Node app. 
- Hosting your front end you have many options. Choose one from the list below:  
  - [Render](https://render.com/)
  - [AWS S3](https://github.com/multiplegeorges/vue-cli-plugin-s3-deploy)    
  - [Netlify](https://www.netlify.com/docs/redirects/#history-pushstate-and-single-page-apps)
  - [Heroku](https://devcenter.heroku.com/articles/heroku-cli)
  - [Surge](http://surge.sh/)


# Bonus Functionality For the Swatches Manager
The below features can be added to get bonus points for added functionality: 
- Add the ability for a swatch to have `multiple images`. Each swatch can view multiple images.
- Add the ability for swatches to be turned on and off i.e. `Active/inactive`.