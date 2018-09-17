# NgxStarter

This is a sample Angular boilerplate code base that can be used for as a guide for setting up your project.

## What's on this boilerplate project?
- **Sass/SCSS setup**. Sass files inside `src/sass` folder. Follow the [Sass 7-1 Pattern](https://sass-guidelin.es/#architecture) when organizing the Sass project.
- **Local build settings**.
    - **Sourcemaps and CSS**. When running a development server, sourcemaps are generated and CSS rules are extracted from global styles onto css files instead of JavaScript ones.
    - **Watch**. File watching is enabled when building locally.
    - **Output Directory**. Output directory is not removed if it exists.

## Dev and Prod Environments

| | ng build | ng build --prod --build-optimizer |
| :- |:-:| -:|
| Environment   | environment.ts | environment.prod.ts |
| Cache-busting | Only images referenced in css | All build files |
| Source maps | Generated | Not generated |
| Uglification | No | Yes |
| Bundling | Yes | Yes |
| Code Splitting | Yes | Yes |
| AOT | No | Yes |
| Tree Shaking | No | Yes |


## Create the Angular project

Run this Angular CLI command.
This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.7.4.

```bash
ng new <my-project-name> --style scss --routing
```

### Build

Run this command to build the project.

```bash
npm run build
ng build --sourcemaps --extract-css
```
The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

### Development server

Run this command for a dev server.

```bash
npm start
ng serve --sourcemaps --extract-css
```

Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

### Code scaffolding

Run to generate a new component.

```bash
ng generate component <component-name></component-name>
ng generate directive|pipe|service|class|guard|interface|enum|module
```

### Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

### Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

### Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
