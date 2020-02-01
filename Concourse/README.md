[![Build Status](https://travis-ci.com/Hacklor/PubQuiz.svg?branch=master)](https://travis-ci.com/Hacklor/PubQuiz)
[![codecov](https://codecov.io/gh/Hacklor/PubQuiz/branch/master/graph/badge.svg)](https://codecov.io/gh/Hacklor/PubQuiz)

# PubQuiz
With this App you can play a PubQuiz game. Just select a Quiz and play!

*Note: It is developed with Mobile Devices in mind.*

## Prerequisites
- [asdf](https://asdf-vm.com/#/core-manage-asdf-vm)

## Setup
`asdf` automatically installs the correct nodejs and yarn versions

```bash
asdf install
yarn install
```

## Available Scripts
In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

## Heroku Deployment
[Heroku URL of Pubquiz](https://starry-sky-pubquiz.herokuapp.com/)

The `master` branch is automatically deployed on Heroku when all the checks (Travis CI) have passed.
To manually deploy use the Heroku CLI tools and GIT.

```bash
git push heroku master
```
