## Learning Babel

The goal of this project is to be able to explain how babel is used, by creating a very simple babel/js CLI project.
I've deliberately used Babel without a build tool such as webpack, so that I can concentrate on Babel.

I've used the Babel setup instructions as a guide.

[Babel Setup](https://babeljs.io/setup#installation)

### How to Install

Install dependencies:

```console
$ npm install
```

### How to Run

Run the build script:

```console
$ npm run build
```

The output from the babel compilation should then appear in the lib folder.

### User Stories

As a Developer,  
I want to compile my ES6 javascript to previous versions,  
So that it will run in any browser.  

As a Developer,
I want to comppile my jsx React code,
So that it will run in a browser.

### Learning Notes

- The most basic setup involves just a config file (.babelrc), which specifies which presets to use, and a script or command to run babel.
- package-lock.json should be commited (ie not ignored).
- node_modules should be ignored by git.
- "git reset" can be used to unstage files which haven't been commited yet.
- "Plugins" in babel are very specific, and cover e.g. just ES6 arrow functions.
- "Presets" in babel are collections of babel plugins which have been bundled together. I've used the popular ENV preset, which collects together all the ES6 plugins, which seems to work with my test js file.

### Credits

[Babel Presets](https://blog.jakoblind.no/babel-preset-env/)
