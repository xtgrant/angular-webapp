# AngularWebapp

This project was generated with [angular-cli](https://github.com/angular/angular-cli) version 1.0.0-beta.24.

## Dependencies
You must have node and npm installed to run. To easily serve, build, or generate components, services, pipes or any supported features you can use angular-cli. To install the angular client from anywhere in the console just run:
```
npm install -g angular-cli
```

## Installation
First you need to clone the repo using SSH or HTTP. It will install into a folder called angular-webapp.
```
git clone git@github.com:thebaron24/angular-webapp.git
```

Then Change directories to the angular webapp.
```
cd angular-webapp
```

Now you need to install the node module dependencies. Inside the angular-webapp folder run:
```
npm install
```

After all of your dependencies are loaded you can run the project with angular-cli. If you havent already run:
```
npm install -g angular-cli
```

Once you have the angular client installed just run this to serve the webapp:
```
ng serve
```

You can see your new angular 2 webapp at:
```
http://localhost:4200
```

## Theming
Currently angular-webapp comes with two choices for theming pre-installed: [material2](https://github.com/angular/material2) and the css only for [bootstrap4](https://github.com/twbs/bootstrap). This allows the developer to choose the option best suited for thier project and begin coding right away. You can remove either after you have made your decision.

### Bootstrap 4
Bootstrap 4 can be customized by modifying the sass files in the bootstrap folder within the node_modules folder

Once you have installed angular-webapp node module dependencies by running `npm install` in the installation section above, you can navigate from the main angular-webapp folder `to node_modules/bootstrap` folder and run `npm install` from your command line to install the Bootstrap 4 dependencies. You only need to do this if you want to customize Bootstrap or if you want to use the new flex grid (which is highly recommended).

Once the dependencies have finished installing open the `_variables.scss` file that resides inside the bootstrap scss folder. Find the variable ``$enable-flex:`` and change it to `true`. Precompile the css with the changes by running `grunt` from the top level of the bootstrap folder. The angular-webapp project already points to the newly compiled css.

You can modify the other variables inside `_variable.scss` to customize the bootstrap theme as well, or follow your favorite bootstrap theming guide.

### Material 2
Theming [Material2](https://github.com/angular/material2) is a little easier. Open the `style.scss` file inside the angular-webapp/src folder and follow the guide set up for you at [Material2 Theming](https://github.com/angular/material2/blob/master/guides/theming.md). For some color choices to start with check out the color guide at [Material2 Theme Colors](https://material.io/guidelines/style/color.html).

## Development server
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive/pipe/service/class/module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Deploying to Github Pages

Run `ng github-pages:deploy` to deploy to Github Pages.

## Further help

To get more help on the `angular-cli` use `ng help` or go check out the [Angular-CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
