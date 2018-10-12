# Angular Project Template

I come up with the idea to create the project with the following the main reason:
I used Angular CLI a lot to create a new project.  Although Angular CLI is great, a new generated project does not contain all ingredients I wanted.  Therefore, I created the project to keep it as my new Angular project template.

The project shows how Angular (6) can combines with following technology:
* SCSS: Use SCSS rather than css
* Bootstrap: Use Bootstrap rather than create styles from scratch
  * Picked up "Navbar example" as an example for the home page
  * Also used ng-bootstrap
* Prettier: Opinionated Code Formatter
* Firebase
* VS Code: Contain .editorconfig

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
* Firebase:
  * If you are not using Firebase, you can simply remove firebase.json and .firebaserc
  * If you are using Firebase, you just need to open .firebaserc and update Firebase project name used
* VS Code: If you are using other code editing tool, you can remove .editorconfig
* Bootstrap: If you need JS of Bootstrap, you may install jQuery `npm install jquery@1.9.1 --save`

## Development

### Start a dev server

Run `npm run start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.

### Build

Run `npm run build` to build the project. The build artifacts will be stored in the `dist/` directory. Use `npm run build:prod` for a production build.

### Test

* Run `npm run test` to execute the unit tests via [Karma](https://karma-runner.github.io).
* Run `npm run test:cov` to execute the unit tests plus get test coverage
* Run `npm run e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).