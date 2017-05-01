# Sample App: Force.com Development with Heroku

## Button Deploy

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Manual

### Clone this code to your local computer

    $ git clone https://github.com/jesperfj/sfdx-simple.git

### Create a Heroku app

    $ heroku create

### Set the Force.com buildpack

    $ heroku buildpacks:set https://github.com/jesperfj/force-buildpack.git

### Add the addon

    $ heroku addons:create force-devhub:test

### Link you Heroku account and Force.com Dev Hub

Go to https://force-devhub.herokuapp.com and link your Developer Hub account to your Heroku Personal Account or one of your teams. If you link it to a team, then anyone who can create apps and addons on that team can authorize those apps to use the Developer Hub.

### Push

    $ git push heroku master

### Test

    $ heroku run test
