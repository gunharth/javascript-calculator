# calculator WIP

A JavaScript calculator

[Project Outline](https://gitlab.web.fh-kufstein.ac.at/WCIS18/pww-unterlagen/tree/master/uebung)

## Installation

Clone the repository
```
git clone git@gitlab.web.fh-kufstein.ac.at:gunharth/calculator.git
````
cd into the directory
```
cd calculator
````
Install all dependencies. This also installs all dependencies for web and api
```
npm install
```
Start and open the frontend on localhost:3000. Start the backend on localhost:3001.
```
npm start
```

## Development
### Frontend

cd into the directory web
```
cd web
````
Compile src/app.js and src/app.scss to the public folder
```
npm run dev
```
Start LiveReload and listen to changes  (Get LiveReload Browser extension: https://chrome.google.com/webstore/detail/livereload)  
Note: Keep dev tools open and disable cache in Chrome dev tools under the Network tab for cache busting
```
npm run watch
```
Compile and minify all assets for production
```
npm run prod
```

## Features
- separation of front-end (web) and back-end (api)
- basic and advanced operations
- history of calculations is shown in front-end (non-persistent)
- history of calculations is saved on the server side under api/calculations.txt
- uses jQuery
- sass setup with normalize.css, fontawesome and Google Roboto font.
- style preferences are saved into localStore
- uses Laravel-Mix for compilation and minification
- calculations are performed by the nodejs/express server through json post requests
- Keyboard support (add tooltip to buttons!)
- removed native Math functions and now uses decimal.js


## Further Options & todos
### Functionality
- use Typescript? Maybe server-side?

### Design
- implement Bootstrap
- show tooltips on buttons
