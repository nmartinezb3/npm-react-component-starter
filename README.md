# npm-react-component-starter

Project sample prepared for create and publish React components on [npm](https://www.npmjs.com/)


## Features
- Webpack for building
- Sass ready (sass-loader). Just ```import 'your/sass/files.scss``` from your components
- ES2016 enabled (babel loader).

## Steps
1. Clone the repo
2. Change package name, author, etc in package.json
3. Install all dependencies: ```npm install```
4. Create your components under ```src/components/```
5. Export them from from src/index.js:
6. Make a build: ```npm run build```
7. Publish to npm: ```npm publish```  (You must have an npm account)
8. You are ready to install the package with ```npm install my-react-components```


## Preview components during develop
In order to preview the component during development:
1. Run ```npm start``` wich runs webpack in watch mode
2. Create a symlink of the package: ```npm link```
3. Create a new react project, for example with [create-react-app](https://github.com/facebookincubator/create-react-app)
4. Install the package from the symlink: ```npm link my-react-components```
5. Import the component: ```import { MyComponent } from 'my-react-components'```
6. Use it! ```<MyComponent />```

