# npm-react-component-starter

Project sample prepared for publishing React components on npm


## Features
- Use webpack for building component
- Sass enabled (sass-loader)
- ES2015 enabled (babel)

## Steps
1. Clone the repo
2. Change package name, author, etc in package.json
3. ```npm install```
4. Create your components under ```src/components/```
5. Export them from from src/index.js:
6. Run ```npm run build```
7. Run```npm publish```  (You must have an npm account)


## Preview components during develop
In order to preview the component during development:
1. Run ```npm start``` wich runs webpack in watch mode
2. Create a symlink of the package: ```npm link```
3. Create a new react project, for example with create-react-app
4. Install the package from the symlink ```npm link my-react-components```
5. Import the component ```import { MyComponent } from 'my-react-components'```

