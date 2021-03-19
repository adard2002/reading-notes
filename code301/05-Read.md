# Reading 05 Notes

[Home](README.md)
# 

# Installing Heroku
1. in your Ubuntu 16+ run the following command in your terminal: sudo snap install heroku --classic
2. Login to Heroku by simply typing: heroku login in your terminal. This will take you to a webpage where you create or login to your account. 
3. You are going to want to make sure you have node, npm, and git installed. you can do this by entering the following commands: node --version, npm --version, and git --version
4. After you have made sure you have those three installed you are going to want to clone a local version of the sample application that you can then deploy to Heroku. run the following commands in your terminal: git clone https://github.com/heroku/node-js-getting-started.git and cd node-js-getting-started. 
5. To be able to deploy the heroku app. Type in the terminal: heroku create. After that type in: git push heroku main.
6. To make sure the app is deployed, make sure that at least one instance of the app is running: heroku ps:scale web=1. To open the app just type: heroku open
7. To view information about your running app use: heroku logs --tail



## What is Node.js
Node.js is a cross-platform runtime environment which allows you to build some server-side and networking applications.