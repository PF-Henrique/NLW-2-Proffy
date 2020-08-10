<h1 align="center">
    <img alt="proffy-landing" src="https://github.com/PF-Henrique/NLW-2-Proffy/blob/master/.github/mockup.png" />
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
  <a href="#-Contributing">🤝 Contributing</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-license">📚 License</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
    
</p>

<div align="center">
Acesse os Readmes com passo a passo, divididos em Front-end, Back-end e Mobile:  <br><br>

💻 **Acesse o Front-end [aqui](https://github.com/PF-Henrique/NLW-2-Proffy/tree/master/web)** | 
🖥 **Acesse o Back-end [aqui](https://github.com/PF-Henrique/NLW-2-Proffy/tree/master/server)** | 
📱 **Acesse o Mobile [aqui](https://github.com/PF-Henrique/NLW-2-Proffy/tree/master/mobile)** |
</div>

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

>The above command will install all third party dependencies used. If you want to install manually all the dependencies follow the steps bellow

```ps
# Entering in server directory
$ cd server

# Installing depencies
$ yarn add @types/cors -D
$ yarn add @types/express -D
$ yarn add ts-node-dev -D
$ yarn add knex
$ yarn add sqlite3
```

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


>The above command will install all third party dependencies used. If you want to install manually all the dependencies follow the steps bellow

```ps
# Entering in web directory
$ cd web

# Installing depencies
$ yarn add @types/react-router-dom -D
$ yarn add axios
```

To start the server you need the database, to make migrations use the command:

```
$ yarn knex:migrate
```
>The above command is a custom command made on `package.json` file. (Ln 8, Col 5)

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

>The above command will install all third party dependencies and fonts used. If you want to install manually all dependencies and fonts used. follow the steps bellow

```ps
# Installing fonts used
$ expo install expo-font @expo-google-fonts/archivo
$ expo install expo-font @expo-google-fonts/poppins

# Installing dependecies required
$ yarn add @react-navigation/native
$ expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view
$ yarn add @react-navigation/stack
$ yarn add @react-navigation/bottom-tabs
$ yarn add axios
$ expo install @react-native-community/async-storage
```

#### 5. `yarn start` or `npm run start` 🎲

To run the tests, after the dependencies are installed, run `yarn test`.

`yarn test:watch` to keep testing observing changes.

`yarn test:coverage` to generate the test coverage report in the files.

## 🤝 Contributing  

There are many forms to contribute with the project, first of all you can give this github repo a Star.

If you want do help with the code follow the steps bellow

```ts
# Fork using GitHub official command line
# If you don't have the GitHub CLI, use the web site to do that.
$ gh repo fork PF-Henrique/NLW-2-Proffy

# Clone your fork
$ git clone {your-fork-url}
$ cd proffy

# Create a branch with your feature
$ git checkout -b {branch-name}

# Make the commit with your changes
$ git commit -m 'Feat: {feature-name}'

# Send the code to your remote branch
$ git push origin {branch-name}
```

Then send a Pull Request that will be analyzed and approved if it helps with the project

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
