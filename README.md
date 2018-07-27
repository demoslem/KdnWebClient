# KdnWebClient

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.7. It contains an [Angular 5.2](https://angular.io) client app and (as git submodule) an [Express.js](http://expressjs.com) based web server that is able to serve the client app. Both, client and server app are written in [TypeScript](https://www.typescriptlang.org/) on the [Node.js](https://nodejs.org/en/) development platform. The Angular client app uses [Angular Material 5.2](https://material.angular.io) for UI components.

## Install

Get the code
```shell
git clone --recursive https://devrepo.krohnegroup.com/gitlab/Testing/Tools/KdnWebClient.git
cd KdnWebClient
```

### Production environment (use-only)

Install all required runtime dependencies.
```shell
npm install --production
```

If not already done, enable the production environment on your machine:
  * Linux: `export NODE_ENV=production`
  * Windows: `set NODE_ENV=production`

Start the Express.js web server.
```shell
node dist/server/bin/www.js --path ./KdnWebServer
```

Navigate to `http://ip_address_of_your_machine:4300`, the Express.js web server serves the Angular client app.

### Development environment (build & use)

Install all runtime and development dependencies.
```shell
npm install
```

The development enviroment is the default environment. If the production environment was previously enabled on your machine, disable it:
  * Linux: `export NODE_ENV=`
  * Windows: `set NODE_ENV=`
  
Start a webpack development server for the Angular client app.
```shell
npm start
```

Navigate to `http://localhost:4200`. The Angular client app will automatically rebuild & reload if you change any of the source files. The Express.js web server is available on `http://localhost:4300` and is also automatically rebuilt & reloaded on soure file changes.

#### Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

#### Production build

Run `npm run build` to create a new production build of the Angular client app and the Express.js web server.
Run `npm run server:build` to create a new production build of the Express.js web server only.

## Running unit tests

~~Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).~~
Not supported yet.

## Running end-to-end tests

~~Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).~~
Not supported yet.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
