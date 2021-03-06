# Nuxt & Firebase(Hosting and Functions SSR), RTDB, Google Auth SNS Example

![image](https://user-images.githubusercontent.com/6993514/34213748-743d6dec-e5e3-11e7-9b1d-a69a12a5637b.gif)

## Requirements

Need the following environment variables.

![Image](https://user-images.githubusercontent.com/6993514/34213945-27f5607e-e5e4-11e7-9761-d5e38e8cf209.png)

```bash
export APIKEY=
export AUTHDOMAIN=
export DATABASEURL=
export PROJECTID=
export STORAGEBUCKET=
export MESSAGINGSENDERID=
```

recommendation: [direnv/direnv](https://github.com/direnv/direnv)

## Build Setup

``` bash
# install dependencies
$ yarn

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start
```

## Deploy to Firebase

This application can also be launched with the normal Node.js application.
However, by using Firebase Hosting and Firebase Functions, it can be used efficiently in a serverless environment.

### setup project

```
$ yarn firebase init
```


### setup env

```bash
firebase functions:config:set environment.apikey=""
firebase functions:config:set environment.authdomain=""
firebase functions:config:set environment.databaseurl=""
firebase functions:config:set environment.projectid=""
firebase functions:config:set environment.storagebucket=""
firebase functions:config:set environment.messagingsenderid=""
```

### deploy

```
$ yarn deploy
```
