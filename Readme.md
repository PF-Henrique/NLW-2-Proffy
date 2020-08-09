<h1 align="center">
    <img alt="proffy-landing" src="https://github.com/PF-Henrique/NLW-Proffy-Rocketseat/blob/master/1%20-%20NLW%20%2302%20-%201400x900.jpg" />
</h1>

<p align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/azagatti/template-react-typescript?style=plastic">

  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/azagatti/template-react-typescript?style=plastic">

  <img alt="Repo size" src="https://img.shields.io/github/repo-size/azagatti/template-react-typescript?style=plastic">

  <a href="https://github.com/AZagatti/template-react-typescript/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/azagatti/template-react-typescript?style=plastic">
  </a>

  <a href="https://github.com/AZagatti/template-react-typescript/issues">
    <img alt="GitHub issues" src="https://img.shields.io/github/issues/azagatti/template-react-typescript?style=plastic">
  </a>

  <a href="https://github.com/AZagatti/template-react-typescript/pulls">
    <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/azagatti/template-react-typescript?style=plastic">
  </a>
</p>

<h4 align="center">
  Next Level Week #2
</h4>

<p align="center">
  <a href="#-about-project">ℹ️ About</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-tecnologias-and-packages">💻 Tecnologies</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-layout">🔖 Layout</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-getting-started">🚀 Getting started</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-customize-">🎯 Customize</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-license">📚 License</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
    
</p>

<br>

## ℹ️ About Project

<div align="center">

  <p align="center">
    
Proffy is a project proposal that facilitates the lives of teachers and students in their day-to-day learning, making it possible for students to view available teachers to teach a subject of interest and to contact them via WhatsApp, or in the case to be a teacher, he can register and offer his study services to new students.
  </p>

</div>

## 💻 Tecnologies and Packages

Este projeto contém as seguintes tecnologias:

#### 🔨 Tecnologies

| Type                | Support   |
|---------------------|:---------:|
| [React](https://reactjs.org)                          | ✔         | 
| [TypeScript](https://www.typescriptlang.org/)         | ✔         |
| [Styled Components](https://styled-components.com/)   | ✔         |
| [Expo](https://expo.io/)                              | ✔         |

#### 📦 Packages

| Type                | Support   |
|---------------------|:---------:|
| [React DOM](https://pt-br.reactjs.org/docs/react-dom.html)        | ✔         |
| [React Router Dom](https://reacttraining.com/react-router/web/)   | ✔         |
| [Dotenv](http://npmjs.com/package/dotenv)                         | ✔         |

In the dev dependencies the Webpack, Jest, Fast Refresh, Eslint and Prettier are configured.

## 🔖 Layout

To access the layout use [Web](https://www.figma.com/file/W7X5HgkYaruZnUVKHj6Uz4/Proffy-Web) or [Mobile](https://www.figma.com/file/FSQdUUY3n8YZeLkpZTJYBT/Proffy-Mobile).

## 🚀 Getting started!

First of all you need to have `node` and `yarn`(or `npm`) installed on your machine.

_If you decide to use npm don't forget to delete yarn.lock in folders_

Press the `Use this template` button on Github and create your own repository.

Clone your repo to your local machine.

#### 1. Git cloning my repo 🎲

```sh

git clone https://github.com/PF-Henrique/NLW-Proffy-Rocketseat.git

```
#### 3. Arquiteture 🎲

````.
├── bin
├── node_modules
├── public
├── src
│   ├── cofig
│   │   └── connection.js
│   ├── controller
│   │   └── user.js
│   ├── model
│   │   └── user.js
│   ├── routes
│   │   └── user.js
│   └── service
│       └── user.js
├── views
├── package-lock.json
├── package.json
└── server.js
````
### 📦 Run API

```bash
# Go to server folder
$ cd proffy-nlw/server

# Install Dependencies
$ yarn install

# Run Aplication
$ yarn start
```
Access API at http://localhost:3333/

### 💻 Run Web Project

```bash
# Go to web folder
$ cd proffy-nlw/web

# Install Dependencies
$ yarn install

# Run Aplication
$ yarn start
```
Go to http://localhost:3000/ to see the result.

### 📱 Run Mobile Project

To run the mobile project you need a cellphone with the app of [expo](https://play.google.com/store/apps/details?id=host.exp.exponent) instaled or a emulator android/ios.
<br />
After, fork this repository and clone to your machine. Inside of the project's folder run the following commands:

```bash
# Go to mobile folder
$ cd proffy-nlw/mobile

# Install Dependencies
$ yarn install

# Run Aplication
$ yarn start
```
Aferter read the QRCode with the app of [expo](https://play.google.com/store/apps/details?id=host.exp.exponent) or run on emulator.

#### 5. `yarn start` or `npm run start` 🎲

To run the tests, after the dependencies are installed, run `yarn test`.

`yarn test:watch` to keep testing observing changes.

`yarn test:coverage` to generate the test coverage report in the files.

#### 6. Open in navigator of your preference 🎲

<h1 align="center">
    <img alt="proffy-landing" src="https://github.com/PF-Henrique/NLW-Proffy-Rocketseat/blob/master/thumbnail.png" />
</h1>

## 🎯 Customize

You have the freedom to change everything in your project, from the settings of Webpack, Jest and even create new structures.

Example of a private route:

<details>
  <summary>Route.tsx</summary>

```ts
import React from 'react';
import {
  Route as ReactDOMRoute,
  RouteProps as ReactDOMRouteProps,
  Redirect,
} from 'react-router-dom';

import { useAuth } from '../hooks/auth';

interface RouteProps extends ReactDOMRouteProps {
  isPrivate?: boolean;
  component: React.ComponentType;
}

const Route: React.FC<RouteProps> = ({
  isPrivate = false,
  component: Component,
  ...rest
}) => {
  const { user } = useAuth();
  // You can store user data in another way and only retrieve it here

  return (
    <ReactDOMRoute
      {...rest}
      render={({ location }) => {
        return isPrivate === !!user ? (
          <Component />
        ) : (
          <Redirect
            to={{
              pathname: isPrivate ? '/' : '/dashboard',
              state: { from: location },
            }}
          />
        );
      }}
    />
  );
};

export default Route;
```

</details>

To create new paths with `@folder` you must change tsconfig.json and jest.config.js by adding the following lines:

In tsconfig.json add lines inside the `paths` as in the example:

```json
"@styles/*": ["styles/*"],
"@newfolder/*": ["newfolder/*"]
```

In jest.config.js add lines inside the `moduleNameMapper` as in the example:

```js
'^@styles/(.*)$': '<rootDir>/src/styles/$1',
'^@newfolder/(.*)$': '<rootDir>/src/newfolder/$1'
```

---
## 🐛 Issues

Feel free to **file a new issue** with a respective title and description on the the [Proffy](https://github.com/PF-Henrique/NLW-Proffy-Rocketseat/issues) repository. If you already found a solution to your problem, **i would love to review your pull request**!

## 📚 License
<p align="justify">
This project is licensed under the <a href="https://github.com/PF-Henrique/NLW-Proffy-Rocketseat">MIT<a/> License
</p>
    
## 👀 Agradecimentos

* Rocketseat
* Diego Fernandes

---

## ✨ Me

<a href="https:https://github.com/PF-Henrique/">
  <img src="https://avatars1.githubusercontent.com/u/48561196?s=460&u=5b39cdc8c6d447868ca0caac900f1ee7a1793962&v=4" width= "50px;" height= "50px;" alt="Avatar"/>
  <br />
 <sub>
  <b>
    Pedro Ferreira
  </b>
</sub>
</a> 
<a href="<a href="https:https://github.com/PF-Henrique/" title="proffy">🚀👩‍🚀</a>
<br />

Made with 💙 by Pedro Ferreira 👋 [Talk to me!](https://www.linkedin.com/in/pedro-ferreira-148503b8/) :octocat:
