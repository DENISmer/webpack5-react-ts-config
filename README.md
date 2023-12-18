Hi! 
## Initially, a project was made according to [this article](https://habr.com/ru/articles/597389/), and also described in [this repository](https://github.com/eadenink/webpack-5-react-config) and [this](https://github.com/DENISmer/webpack5-react-config), but the configuration described in these links did not suit me for several reasons:

1. no TS support.
1. no support for scss modules.
1. and etc.

## This webpack5 configuration will allow you to use the following core technology stack:
1. React
1. TS
1. CSS
1. SCSS
1. SCSS modules
1. support for the following file extensions:
(png|jpe?g|gif|svg|webp|ico) and (woff2?|eot|ttf|otf)
1. and etc.

## All you need to use this config:

1. clone this repository
```
git clone https://github.com/DENISmer/webpack5-react-ts-config
```
2. installing dependencies
```
npm install
```
3. run the required script:
```js
    "start": "cross-env SERVE=true webpack serve --mode development" // run dev-server
    "build": "webpack" // simple build
    "build-prod": "webpack --mode=production" // create production build
    "local-deploy": "npx serve -s build" // local deploying (if a build was previously made)
    "deploy": "gh-pages -d build" // deploying on gh-pages (if a build was previously made)
    "clean": "rd /s /q build" // clean the build derictory
    "cb-dep": "npm run clean && npm run build-prod && npm run deploy" // clean ./build -> create production build -> deploy on gh-pages
```
