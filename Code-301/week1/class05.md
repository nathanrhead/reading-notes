# Code 301 | Heroku: Getting Started with Node

## Class 05 Reading Notes

### ["Getting Started on Heroku with Node.JS"](https://devcenter.heroku.com/articles/getting-started-with-nodejs)

I. Heroku Setup: takes you through a step-by-step process to download heroku via the command line and to create an account and log in.

II. Deploy a sample heroku site: step-by-step instructions on deploying a sample heroku site, cloned from github, to the interwebs. 

III. Procfile

- "A text file in the root directory of your application, to explicitly declare what command should be executed to start your app."

- Example: "web: node index.js"

- "This declares a single process type, web, and the command needed to run it. The name web is important here. It declares that this process type will be attached to the HTTP routing stack of Heroku, and receive web traffic when deployed.

- "Procfiles can contain additional process types. For example, you might declare one for a background worker process that processes items off of a queue."

IV. Scaling the app

- The sample app is running on a "single web dyno," a container that runs the procfile command.

- Free dynos, like this one, sleep after 30 minutes of inactivity and require a few seconds to wake up; they also have monthly quotas.

- Upgrade to a hobby or dyno type, as required, to scale it.

V. Declaring app dependencies

- "Heroku recognizes an app as Node.js by the existence of a package.json file in the root directory. For your own apps, you can create one by running npm init --yes."

- "The package.json file determines both the version of Node.js that will be used to run your application on Heroku, as well as the dependencies that should be installed with your application."

VI. Running your app locally: from the CLI, run "heroku local web" and open http://localhost:5000. 

VII. Pushing local changes

- git add .; git commit -m""; git push heroku main;

- heroku open filenamej

VII. Provision add-ons: "Add-ons are third-party cloud services that provide out-of-the-box additional services for your application, from persistence through logging to monitoring and more." You have to add a credit card to continue.

[<--back](301week1.md)

[<--home-->](../../README.md)
