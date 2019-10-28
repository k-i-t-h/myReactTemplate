This is my React Template with no support for OFFLINE(ServiceWorker)

________________________________________________________________________________________
									React.js Checklist 
________________________________________________________________________________________


*ADD REACT TO EMPTY FOLDER

*Use following syntax on VScode(terminal) to install react on the current empty Folder 
COPY BELOW

npx create-react-app .

________________________________________________________________________________________
________________________________________________________________________________________

*OPEN DEV SERVER

*To run dev server open VScode(terminal)
COPY BELOW 

npm start
________________________________________________________________________________________________________________________________________________________________________________

***CLEAN UP***


1) (INDEX.HTML)

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <meta
      name="description"
      content="Web site created using create-react-app"
    />
    <link rel="apple-touch-icon" href="logo192.png" />

    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />

    <title>my-app-play</title>
  </head>
  <body>
    <div id="root"></div>
  </body>
</html>



*Should have <div>id=“root”</div> inside the body tag!!!
________________________________________________________________________________________

2) (INDEX.JS)

import React from "react";
import ReactDOM from "react-dom";
import App from "./App";

ReactDOM.render(<App />, document.getElementById("root"));


**Above is ServiceWorker disabled template for (INDEX.JS)

(If need frameworks like bootstrap etc. add it to header or index.html)
(If project requires offline environment then do not edit/rm ServiceWorker syntax.) otherwise (INDEX.JS) should look similar to above.

** DELETE (INDEX.CSS) and IMPORTS
** DELETE LOGO.SVG and IMPORTS
________________________________________________________________________________________

3) (APP.JS)

import React, { Component } from "react";
import "./App.css";

class App extends Component {
  render() {
    return (
      <div>
        {/* 
	   <Header />
        <MainContent />
        <Footer /> 
		*/}
      </div>
    );
  }
}

export default App;



**ABOVE (APP.JS) should look like this
________________________________________________________________________________________

4) (APP.CSS)

* {
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}

a {
  color: black;
  text-decoration: none;
}

**EDIT (APP.CSS) to specific needs or use template below for starters
________________________________________________________________________________________

5) components (Folder)

Create ‘components folder’ inside the ‘src folder’
and create all ‘component files’ inside.


END OF CHECKLIST
________________________________________________________________________________________






This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

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

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
