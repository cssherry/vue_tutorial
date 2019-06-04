# Creating New Project

Following [official tutorial](https://vuejs.org/v2/guide/)

## Compatability
- Does not support IE8
- Debug with [Vue Devtools](https://github.com/vuejs/vue-devtools#vue-devtools)
  - Chrome: https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd

## Installation
- `npm install vue` or `npm install -g @vue/cli` for [cli](https://cli.vuejs.org/)
-

## Build
- Gulp vs browserfy vs webpack comparisons:
  - https://www.cleveroad.com/blog/gulp-browserify-webpack-grunt
  - https://www.toptal.com/front-end/webpack-browserify-gulp-which-is-better
- Using webpack

## Starting Projects
- Create vue app with `vue create APP_NAME`
    - Took a really long time to create new project
- Options
    - Babel
    - TypeScript
        - class-style component syntax: similar to angular, define components as classes with propertyies and decorators describe component (https://alligator.io/vuejs/typescript-class-components/)
        - Use babel along typescript (allow auto-detect polyfills, transpile JSX)
        - Benefits: reduce error due to compile type checking, help communicate api's expected parameters and return values. Some of these benefits are also communicated with good tests
    - Progressive Web App (user service workers for offline support)
    - Router (For single page app)
        - history mode (instead of hash -- needs to have fallback index.html to be served in case url routing doesn't match in server)
    - Vuex (for data binding)
    - CSS Pre-processor (for different CSS)
        - Sass/SCSS dart-sass: primary implementation of Sass
        - Sass/SCSS node-sass
    - Linter/Formatter
        - ESLint (preferred now): default for js
        - TSLint: for typescripting, but going to be focusing on improving typescript within ESLint (https://medium.com/palantir/tslint-in-2019-1a144c2317a9)
    - Unit Testing (https://medium.com/welldone-software/an-overview-of-javascript-testing-in-2018-f68950900bc3)
        - Mocha + chai: need libraries for assers, very flexible
        - Jest: Used for react, really fast due to parallel testing, snapshot testing
    - E2E Testing (end-to-end testing)
        - Cypress
        - Nightwatch

## Running Project

- `npm run serve` from APP_NAME folder