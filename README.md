# Angular Project Template

The project shows how Angular (6) can combines with following technology:
* SCSS: Use SCSS rather than css
* Bootstrap: Use Bootstrap rather than create styles from scratch
* Prettier: Opinionated Code Formatter

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