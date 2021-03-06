# SampleKarmaJasmineProject

## Test suite command

`npm run tutorTest` runs `ng test --config tutor-karma.conf.js --single-run`, which starts Karma with the `tutor-karma.conf.js` config file, which then searches for any files ending in `.spec.ts` files located in `src/`.

This Karma config has been modified to:

1. Use PhantomJS for headless tests by including `karma-phantomjs-launcher` instead of `karma-chrome-launcher`.
2. Use the Reporter `karma-structured-json-reporter` instead of `karma-jasmine-html-reporter`.

Learners will be prompted to run the standard `ng test` command in a Project, which runs Karma from the standard karma.conf.js and watches and reports test output in Chrome.

## Steps to pass all tests

1. `@does-contain-app-sample` - In `src/app/app.component.html` on line 2, replace `<h1>Hi</h1>` with `<app-sample></app-sample>`.
2. `@contains-h1` - In `src/app/sample/sample.component.ts` on line 17, replace the value of `this.sampleTitle` with `Sample Component Loaded`.
3. `@h1-contains-title` - In `src/app/sample/sample.component.html` on line 2, change the `p` tags to `h1`.

# Default Angular CLI README appears below

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.0.1.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
