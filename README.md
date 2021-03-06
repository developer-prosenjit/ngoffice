# Ngoffice

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.0.1.

## Live demo https://ng-office.firebaseapp.com/

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|module`.

## Build

Run `ng build --aot=true --prod --env=prod` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Precache
sw-precache --root=dist --config=sw-precache-config.js for generate service worker code

## Deploy 
firebase deploy --only hosting

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## Security rule

{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null",
    "tasks": {
        ".indexOn": "done",
          "$uid": {
            ".indexOn": "done",
          }
      }
  }
}
