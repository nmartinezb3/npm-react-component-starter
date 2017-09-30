# npm-react-component-starter

Sample project prepared for create and publish React components on [npm](https://www.npmjs.com/)


## Features
- Use Webpack for building
- Sass ready (sass-loader). Just ```import 'your/sass/files.scss'``` from your components
- ES2016 ready (babel loader).
- Import images from your components (url-loader). Just ```import myImage from 'my/image/dir/my_image.png'``` 

## How to use
1. Clone the repo: ```git clone git@github.com:nmartinezb3/npm-react-component-starter.git```
2. Change package name, author, and all stuff in ```package.json```
3. Install all dependencies: ```npm install```
4. Create your components under ```src/components/```
5. Export them from ```src/index.js```: 
```
import MyComponent from './components/MyComponent';
import MyOtherComponent from './components/MyOtherComponent';

export { 
  MyComponent,
  MyOtherComponent
}
```

6. Make a build: ```npm run build```
7. Publish to npm: ```npm publish```  (you must have an npm account)
8. Install the package from other project: ```npm install my-react-components```
9. Import the components: ```import { MyComponent, MyOtherComponent } from 'my-react-components'```


## Preview components during develop
In order to preview the component during development:
1. Run ```npm start``` wich runs webpack in watch mode
2. Create a symlink of the package: ```npm link```
3. Create a new react project, for example with [create-react-app](https://github.com/facebookincubator/create-react-app)
4. Install the package from the symlink: ```npm link my-react-components``` (check the package name you set in ```package.json```)
5. Import the component: ```import { MyComponent } from 'my-react-components'```
6. Use it! ```<MyComponent />```
7. Everytime you make a change in the component, the changes will be reflected immediately in the preview project.

For more information about npm symlinks, visit https://docs.npmjs.com/cli/link
