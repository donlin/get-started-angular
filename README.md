# Angular Project Template

The project shows how Angular (6) can combines with following technology:
* SCSS: Use SCSS rather than css
* Bootstrap: Use Bootstrap rather than create styles from scratch
  * Picked up "Sticky footer with fixed navbar" as an example for the home page
* Prettier: Opinionated Code Formatter

## Development

### Start a dev server

Run `npm run start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.

### Build

Run `npm run build` to build the project. The build artifacts will be stored in the `dist/` directory. Use `npm run build:prod` for a production build.

### Test

* Run `npm run test` to execute the unit tests via [Karma](https://karma-runner.github.io).
* Run `npm run test:cov` to execute the unit tests plus get test coverage
* Run `npm run e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Used as a project template

If you use the project as a template to create a new project rather than us Angular CLI to generate, you can following steps to create/change:
* Clone the project
* Remove the ".git" folder
* Create a new repository on the command line
  * Run "git init"
  * git commit -m "first commit"
  * git remote add origin https://github.com/...
* Update the following npm settings in package.json
```
{
  "name": "{project name}",
  "version": "{project version}",
  "repository": {
    "type": "git",
    "url": "{repository URL}"
  },
  "license": "MIT",
  ...
}
``` 
* Update angular.json: Replace all "get-started-angular" with the new project name
* Update title in index.html
* Replace favicon.ico