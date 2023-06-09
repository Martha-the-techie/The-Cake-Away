# The-Cake-Away

## Introduction
Congrats on getting through all the material for Phase 3! Now's the time to put it all together and build something from scratch to reinforce what you know and expand your horizons.

The focus of this project is building a Sinatra API backend that uses Active Record to access and persist data in a database, which will be used by a separate React frontend that interacts with the database via the API.

## Requirements
For this project, you must:

Use Active Record to interact with a database.
Have a minimum of two models with a one-to-many relationship.
Create API routes in Sinatra that handles at least three different CRUD actions for at least one of your Active Record models.
Build a separate React frontend application that interacts with the API to perform CRUD actions.
Use good OO design patterns. You should have separate classes for each of your models, and create instance and class methods as necessary.

## Getting Started

## Backend Setup
This repository has all the starter code needed to get a Sinatra backend up and running. Fork and cloneLinks to an external site. this repository to get started. Then, run bundle install to install the gems.

The app/controllers/application_controller.rb file has an example GET route handler. Replace this route with routes for your project.

You can start your server with:

 bundle exec rake server
This will run your server on port http://localhost:9292Links to an external site..

## Frontend Setup
Your backend and your frontend should be in two different repositories.

Create a new repository in a separate folder with a React app for your frontend. cd out of the backend project directory, and use create-react-appLinks to an external site. to generate the necessary code for your React frontend:

 npx create-react-app my-app-frontend
After creating the project locally, you should also create a repository on GitHubLinks to an external site. to host your repo and help collaborate, if you're working with a partner.

## Fetch Example
Your React app should make fetch requests to your Sinatra backend! Here's an example:

fetch("http://localhost:9292/test")
  .then((r) => r.json())
  .then((data) => console.log(data));

## Project Tips
This project is intended to focus more on the backend than the frontend, so try and keep the React side of things relatively simple. Focus on working with Active Record and performing CRUD actions. What are some interesting queries you can write? What kinds of questions can you ask of your data?
Once you have a project idea, come up with a domain model and decide what relationships exist between the models in your application. Use a tool like dbdiagram.ioLinks to an external site. to help visualize your models.
Decide on your API endpoints. What data should they return? What kind of CRUD action should they perform? What data do they need from the client?
Use PostmanLinks to an external site. to test your endpoints.
Use binding.pry to debug your requests on the server. It's very helpful to use a binding.pry in your controller within a route to see what params are being sent.
Use the Network Tab in the Dev ToolsLinks to an external site. in the frontend to debug your requests.

## Links

https://create-react-app.dev/docs/getting-started
https://dbdiagram.io/
https://www.postman.com/downloads/