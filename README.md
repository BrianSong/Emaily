# Emaily - A fullstack project built by React/Redux and Node.js
## *This project is a feedback collection application faced for start-up owner/product manager so that they can collect feedbacks from their own individual users.*

### Teches used in this project:
1. FrontEnd: React/Redux (Redux form).
2. BackEnd Server: Node/Express.
3. Database: MongoDB.
4. Authetication: Google OAuth + Passport JS.
5. Handling Billings: Stripe.
6. Email Provider: SendGrid.
7. Deploy: Heroku.

### Belows are some keypoints that I learned from this emaily project:
* Express/Node API serves as messager between React App (send out HTTP request) and MongoDB.
* `package.json` is a control hub of our project that can be used to define a lot of different dependencies that our project depends upon.
* Node: execute code outside of the brower.
* Express: a library runs in Node runtime that has a collection of helper methods which makes dealing with HTTP traffic requests came from React App easier.
* The incoming HTTP traffic from React App will rush in some port of Node where the Express will use Route Handler to give according responce to Node and up to React App.
* In Node.js, we can not use ES2015 module like *import express from 'express'*, instead, the correct way is *const express = require('express')*.
* Heroku is used to deploy this project, finally, it will return a URL for this project where anyone else can use this URL to use our application instead of *http://localhost:3000* which is only visable for our own local machine.
* If there are some variables that we do not want other engineers to change it, we should name it full capticalize : e.x. CONSTVARIABLE
* Passport JS is used to help OAuth (Google, Facebook, Twitter...) easier. However, it still has some cons:
1. not all automatic.
2. So hard for the user to have a bigger picture about what is going on by just adding some weired code here and there.
3. Need to download multiple passport strategy for mutiple specific provider(Google, Facebook...).
