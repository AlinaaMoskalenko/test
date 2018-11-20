This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## How to create react app

1. In the directory you can run:

### `npm install -g create-react-app`

2. In the next step you must create a new React app called, eg. “test”, using the command below.

### `create-react-app test`

3. Then change to the newly created directory and run the following command to start the application. The start command creates a local development server to run the application.

change directory
### `cd test`

run application in development environment
### `npm start`

4. After checking that the application runs perfectly without any error, you can CREATE a NEW REPOSITORY on GitHub.

5. The next step is to convert the local react project to a git repository.

create a new git repository in you project directory
### `git init`

add all changed file paths to staged changes
### `git add .`

commit all staged changes
### `git commit -m 'initial commit'`

6. After that add the just created GitHub repository as the remote repository and push the code to it using the following commands. It create a default master branch and add all the code to it (eg.):

add remote repository
### `git remote add origin https://github.com/AlinaaMoskalenko/test.git`

pushe local repository to remote repository on GitHub
### `git push origin master`

7. The next step is to install ‘gh-pages’ package using the following npm command:

install gh-pages package
### `npm install --save gh-pages`

8. Then you need to modified the package.json file of the project by adding the following statements (the statements are highlighted):

The “homepage” specifies the host path where you want to host the application. 
The template for the URL is: 

### https://[your-user-name].github.io/[your-repo-name]/

### (eg. https://alinaamoskalenko.github.io/test/)

### “predeploy” specifies the command to build before deployment.
### “deploy” specifies which branch and directory to deploy.

in the top file (after "private": true,)
### `"homepage": "https://alinaamoskalenko.github.io/test/"`

in "scripts":
### `"predeploy": "npm run build",`
### `"deploy": "gh-pages -d build",`

9. The last step is to deploy the application using the following command:

deploy application
### `npm run deploy`

10. Check your site on https://alinaamoskalenko.github.io/test/ (eg.)

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
