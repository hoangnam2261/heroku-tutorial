# Login
heroku login

# clone app
git clone ...

# Create an app on heroku
heroku create %APP_NAME%

# Now deploy your code:

git push heroku main

Heroku recognizes an app as Node.js by the existence of a package.json file in the root directory.

# open app
heroku open

# View application logs:
heroku logs --tail

# Procfile declare what command should be executed to start your app.
```web: npm start```
`web` declares that this process type will be attached to the HTTP routing stack of Heroku, and receive web traffic when deployed.

# check how many dynos are running (a dyno as a lightweight container that runs the command specified in the Procfile.)
heroku ps

# Scale the app
heroku ps:scale web=1

# Run the app locally
heroku local web

# Start a console
heroku run bash
