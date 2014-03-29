[![KOAN](https://raw.github.com/soygul/koan/master/client/img/koan_large.png)](http://koanjs.com/)

[![Build Status](https://travis-ci.org/soygul/koan.png?branch=master)](https://travis-ci.org/soygul/koan)

KOAN Stack is a boilerplate that provides a nice starting point for [Koa](http://koajs.com/), [AngularJS](http://angularjs.org/), and [Node.js](http://www.nodejs.org/) based applications, for full stack JavaScript Web development. It is designed to give you quick and organized way to start developing Web apps with useful modules like [MongoDB](http://www.mongodb.org/), [Passport](http://passportjs.org/), and [Grunt](http://gruntjs.com/) tasks, pre-bundled and configured.

## Getting Started
Make sure that you have Node.js (v0.11 or above) and MongoDB (running on the default port 27017) installed on your computer. To get started with KOAN stack, do following:

```bash
git clone https://github.com/soygul/koan.git
cd koan
npm install
npm start
```

Your application should run on the 3000 port so in your browser just go to [http://localhost:3000](http://localhost:3000). If you want to run tests, simply type:

```bash
npm test
```

## Configuration
All configuration is specified in the [server/config](server/config/) folder, particularly the [config.js](server/config/config.js) file. Here you can hook up any social app keys if you want integration with Twitter, Facebook, or Google.

## Heroku Deployment
Before you start make sure you have <a href="https://toolbelt.heroku.com/">heroku toolbelt</a> installed.

```bash
git init
git add .
git commit -m "initial version"
heroku apps:create
heroku addons:add mongohq
heroku labs:enable websockets
heroku config:add NODE_ENV=production
git push heroku master
heroku open
```

## Receiving updates from upstream
Whenever we update KOAN's repo, you can just fetch the changes and merge them into your project with git.

## Live Example
Browse the live KOAN example on [http://koanjs.com](http://koanjs.com).

## Credits
Client side is entirely based on: [Angular Seed](https://github.com/angular/angular-seed). Server side simply utilizes generally accepted Koa middleware and Node.js best practices.

## The Name
The project name is an acronym for Koa, Angular, and Node. It also is the name for a Zen Buddhist riddle used to focus the mind during meditation and to develop intuitive thinking.

## License
MIT