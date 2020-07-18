# FrontEnd Starter 2020 (React + Redux + Typescript)
![](https://img.shields.io/github/package-json/dependency-version/EgorBedov/FrontEnd-Starter/react/React-Redux-TS?logo=react) ![](https://img.shields.io/github/package-json/dependency-version/EgorBedov/FrontEnd-Starter/redux/React-Redux-TS?logo=redux) ![](https://img.shields.io/github/package-json/dependency-version/EgorBedov/FrontEnd-Starter/dev/typescript/React-Redux-TS?logo=typescript)

![](https://img.shields.io/github/package-json/dependency-version/EgorBedov/FrontEnd-Starter/dev/webpack/React-Redux-TS?logo=webpack) ![](https://img.shields.io/github/package-json/dependency-version/EgorBedov/FrontEnd-Starter/dev/eslint/React-Redux-TS?logo=eslint) ![](https://img.shields.io/github/package-json/dependency-version/EgorBedov/FrontEnd-Starter/dev/sass/React-Redux-TS?logo=sass)

Start your next web application with up-to-date development tools without a struggle of setting them up. Just download it and you're ready to go!

## Setups
List of supported setups:
* React + Redux + Typescript ([branch](/../../tree/React-Redux-TS/))
* React + Redux + Javascript ([branch](/../../tree/React-Redux-JS/))
* Typescript ([branch](/../../tree/TS/))
* Javascript ([branch](/../../tree/JS/))

Default technological stack:
* Webpack module bundler
* ESLint linter
* Babel transpiler
* Sass CSS preprocessor

## Usage
#### Manage repo
1) Mirror repository - [Github tutorial](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/duplicating-a-repository)
2) Choose branch and delete all others 

Manually:
```bash
git branch -d branch_name
git push origin --delete <branch_name>
git push origin :<branch_name>
```
Or delete it on GitHub then do `git fetch --all`
#### Install the setup
```bash
npm install
```

#### Run webpack
```bash
npm start
```

#### Run server
```bash
node src/server.js
```
> Switch to different terminal beforehand

## Clean setup
Run this script to remove default pages, components, models, actions and reducers.
```bash
clean.sh [-ah]
```
> Use -a option to completely delete components, pages, models and static folders

## File structure
You can change the file structure whichever way you want and if you do so, don't forget to change aliases paths in both [Typescript config](../blob/React-Redux-TS/tsconfig.json) and [Webpack config](../blob/React-Redux-TS/webpack.config.json).
```bash
├── dist/               // Auto generated output files
├── node_modules/
├── src
│   ├── components/     // Create your components here
│   ├── models/         // Create your models here
│   ├── pages/          // Create your pages here
│   ├── store
│   │   ├── actions/    // Redux's actions and action creators
│   │   ├── reducers/   // Redux's reducers
│   │   └── store.ts    // Redux's store
│   ├── utils
│   │   ├── assets.d.ts     // Assets declarations (TS)
│   │   ├── constants.ts    // Global constants
│   │   ├── interfaces.ts   // Global interfaces
│   │   └── variables.scss  // Global CSS variables
│   ├── index.html
│   ├── main.scss
│   ├── main.tsx
│   └── server.ts
├── static/             // Static files
├── .babelrc            // Babel config
├── .eslintignore
├── .eslintrc.json      // ESLint config
├── .gitignore
├── clean.sh            // Script to delete old files
├── package.json
├── tsconfig.json       // Typescript config
└── webpack.config.js   // Webpack config
```

## License
[MIT](LICENSE)
