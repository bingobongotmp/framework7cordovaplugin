Based off: vue init AppointmentGuru/webpack-mobile-f7 my-project

Changes from template:

- ```build.js``` moves cordova.js to static on build 

- index.html has script src to cordova


```sh

npm i -g cordova 

npm i -g ios-deploy

npm i

cordova platform add ios

# Add team/certificate in ios

npm run build && cordova build

# Open in xcode, load on device on, deviceready fires but cordova.plugins undefined

```


# f7

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## Mobile

This app is setup to package via Cordova.

**Add whichever platforms you would like to support:**

```
cordova platform add browser
cordova platform add ios
cordova platform add android
```

The following commands are available:

```
cordova-build
cordova-run
cordova-run-ios
cordova-run-android
```

