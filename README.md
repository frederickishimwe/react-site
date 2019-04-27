# Introduction 

This is an implementation of react running directly on a serverless site

## Steps to recreate this repo
## 01
I used the following npm command on git bash to install ‘create-react-app’. This package helps to creates a boilerplate React application to work on.
### `npm install -g create-react-app`

## 02
In the next step I created a new React app called “website” using the command below.
### `create-react-app website`

## 03
Then I changed to the newly created directory and run the following command to start the application. The start command creates a local development server to run the application.

### ` 
    change directory
    cd website
    #run application in development environment
    npm start
 `
## 04
The next step was to convert the local react project to a git repository.
### ` #create a new git repository
$ git init
#add all changed file paths to staged changes
$ git add .
#commit all staged changes
$ git commit -m 'initial commit `

## 05
After that I added the just created GitHub repository as the remote repository and pushed the code to it using the following commands. It created a default master branch and added all the code to it.
### `#add remote repository
$ git remote add origin https://github.com/gurjotmakkar/website.git
#pushed local repository to remote repository on GitHub
$ git push origin master`

## 06
The next step was to install ‘gh-pages’ package using the following npm command:
### `#install gh-pages package
$ npm install --save gh-pages`

## 07
Now I just needed to modified the package.json file of the project by adding the following statements

###`
add json object "homepage":'your git hub pages link'
add two more json objects under the scripts object, predeploy and deploy
"predeploy":"npm run build"
"deploy":"gh-pages -d build"

The “homepage” specifies the host path where you want to host the application. 
The template for the URL is: 
https://[your-user-name].github.io/[your-repo-name]/
“predeploy” specifies the command to build before deployment.
“deploy” specifies which branch and directory to deploy.`
## 08
The last step now was to deploy the application using the following command:
### 
`
#deploy application
$ npm run deploy`

## This basically keeps your code on master, and the build files on gh-pages, make sure your github is hosting from gh-pages branch,

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
