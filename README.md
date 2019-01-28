
# Using SASS Modules In Create React App V2

## Packages

Node-sass: [npm](https://www.npmjs.com/package/node-sass) or [yarn](https://yarnpkg.com/en/package/node-sass)

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Usage

### 1. For styles that are scoped to components, create stylesheets files that end with `.module.scss`

#### Example:
```
.Circle{ 
      background-color: #FFEB3B;
      height: 200px;
      width: 200px;  
      border-radius: 50%; 
      display: inline-table;    
      margin: 10px 0 10px 0;     
      p{
            vertical-align: middle;
            display: table-cell;
            font-size: 16px;
            font-weight: 500;
      }
}
```

### 2. Import the Sass files as objects and use the styling in your components

#### Example:
```
import React from 'react';
import { Circle }  from './YellowCircle.module.scss';

const YellowCircle = () =>{

      return(
            <div className={ Circle }>
                  <p>Yellow</p>
            </div>
      );
}

export default YellowCircle;
```



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



