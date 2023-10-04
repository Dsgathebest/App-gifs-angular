# GifsApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.0.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

## Scripts
Instalarlo de manera local en los proyectos, no global porque podría ser peligroso mal usado, es para poder ejecutar el "del docs" y el otro el "copyfiles"

```
npm install del-cli --save-dev
npm i copyfiles --save-dev
```

```
"ng": "ng",
"start": "ng serve",
"build": "ng build",
"build:href": "ng build --base-href ./",
"build:github":"npm run deleted:docs && npm run build:href",
"watch": "ng build --watch --configuration development",
"test": "ng test",
"deleted:docs": "del docs",
"copy:dist": "copyfiles dist/gifs-app/* ./docs -f"
```

Así se ejecuta al final para generar el build listo para github

```
npm run build:github
```
