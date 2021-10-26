# react-ts-lib
boilerplate for creating a react component library/npm package with typescript

### Structure
Built with yarn 1.22.17 and node v14.17.3
```
|
|- lib/  //build output
|- src/  //library code
|- test/  //create-react-app where components can be viewed/tested
|
```

### Getting Started
- `yarn install` Installs dependencies in both library and create-react-app `test/` directory
- `yarn build` Builds library into `lib` directory
- `yarn start` Starts the create-react-app test application
- `yarn publish` Runs a build then publishes library to npm (Will need to `npm login` first)

### Other Information
In `src/` there is a simple Demo Component.  Any component you wish to test will need to be imported in the `package.json` of the create-react-app (`test`) directory.
It is advised to use the local `link:..` syntax (as done with the Demo Component) instead of publishing and pulling the library down from npm each time.

You **will** need to build the library (`yarn build`) in order for the create-react-app to pickup changes to components.  
