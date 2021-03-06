# Angular, NGXS and Angular Material Starter 
by [@iago_aa](https://twitter.com/iago_aa)

[![license](https://img.shields.io/github/license/Zuiago/angular-ngxs-material-starter.svg)](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/LICENSE) [![All Contributors](https://img.shields.io/badge/all_contributors-8-orange.svg?style=flat-square)](#contributors) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier) [![Build Status](https://travis-ci.org/Zuiago/angular-ngxs-material-starter.svg?branch=master)](https://travis-ci.org/Zuiago/angular-ngxs-material-starter) [![Twitter Follow](https://img.shields.io/twitter/follow/iago_aa.svg?style=social&label=Follow)](https://twitter.com/iago_aa)


![intro](https://raw.githubusercontent.com/Zuiago/angular-ngxs-material-starter/master/meta-assets/intro.png)
![themes](https://raw.githubusercontent.com/Zuiago/angular-ngxs-material-starter/master/meta-assets/themes.png)

## Table of Content

  * [Live Demo](https://https://zuiago.github.io//angular-ngxs-material-starter)
  * [Getting Started](#getting-started)
  * [Useful Commands](#useful-commands)
  * [Make It Your Own](#make-it-your-own)
  * [Learning Materials](#learning-materials)
  * [List of Projects Built Using This Starter](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/BUILT_WITH.md)
  * [Features](#features)
  * [Stack](#stack)
  * [Code of Conduct](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/CODE_OF_CONDUCT.md)
  * [Contributors Guide](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/CONTRIBUTING.md)
  * [Changelog](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/CHANGELOG.md) ( get notified about the newest releases, [follow Release Butler](https://twitter.com/releasebutler) on Twitter )


## Getting started
```bash
git clone https://github.com/Zuiago/angular-ngxs-material-starter.git new-project
cd new-project
npm install
npm start
```

## Useful Commands
  * `npm start` - starts a dev server and opens browser with running app
  * `npm run test` - runs lint and tests
  * `npm run watch` - runs tests in watch mode
  * `npm run prod` - runs full prod build and serves prod bundle
  * `npm run prettier` - runs prettier to format whole code base (`.ts` and `.scss`) 
  * `npm run analyze` - runs full prod build and `webpack-bundle-analyzer` to visualize how much code is shipped (dependencies & application) 

![analzye](https://raw.githubusercontent.com/Zuiago/angular-ngxs-material-starter/master/meta-assets/analyze.png)

## Make It Your Own
When using this starter project to build your own app you might consider some of the following steps:
  
  * use `search and replace` functionality of your favourite IDE to replace `anms` with `<your-app-prefix>`
  * rename project in `package.json` `name` property and set appropriate version (eg `0.0.0` or `1.0.0`)
  * rename app in `src/environments/` files (will be shown in browser tab)
  * delete pre-existing `CHANGELOG.md` (you will generate your own with future releases of your features)
  * delete `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md` and `BUILT_WITH.md` files as they are relevant only if project is open sourced on Github
  * remove or adjust links in the [footer](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/src/app/app.component.html#L79)
  * replace logo in `src/assets` folder ( currently 128 x 128 pixel `png` file )
  * adjust colors in `src/themes/default-theme.scss`
  * create a pull request in the [original repository](https://github.com/Zuiago/angular-ngxs-material-starter/) to update `BUILT_WITH.md` [file](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/BUILT_WITH.md) with a link and short description of your project
  
#### Continuous Integration
Starter project is using [Travis CI](https://travis-ci.org/) for running linters and tests on every commit.
Based on your preferences and needs you can either:

  * not use / use other CI server and delete both `.travis.yml` and `.travis-deploy.sh`
  * create Travis CI account and link it to your projects Github repo and [configure build](https://medium.com/@tomastrajan/continuous-deployment-of-client-side-apps-with-github-pages-travis-ci-10e9d641a889) 
    with `GH_REF` and `GH_TOKEN` environment variables for automatic deployment of releases to Github Pages
  

## Learning Materials
Articles with content that explains various approaches used to build this starter project.

  * [Blog post about Best Practices for Angular CLI](https://medium.com/@tomastrajan/6-best-practices-pro-tips-for-angular-cli-better-developer-experience-7b328bc9db81) used in this starter project
  * [Blog post about Typescript tips for Ngrx reducer code](https://medium.com/@tomastrajan/object-assign-vs-object-spread-in-angular-ngrx-reducers-3d62ecb4a4b0)
  * [Blog post about building responsive layouts with Bootstrap 4 in Angular apps](https://medium.com/@tomastrajan/how-to-build-responsive-layouts-with-bootstrap-4-and-angular-6-cfbb108d797b)
  * [Blog post about configuration of animations during runtime](https://medium.com/tomastrajan/total-guide-to-dynamic-angular-animations-that-can-be-toggled-at-runtime-be5bb6778a0a)
  * [Blog post about unit testing of components with NgRx TestStore](https://medium.com/@tomastrajan/how-to-unit-test-angular-components-with-fake-ngrx-teststore-f0500cc5fc26)
  * [Blog post about Angular CLI budgets](https://medium.com/@tomastrajan/how-did-angular-cli-budgets-save-my-day-and-how-they-can-save-yours-300d534aae7a)

#### Theming 

  * [Blog post](https://medium.com/@tomastrajan/the-complete-guide-to-angular-material-themes-4d165a9d24d1)
  * [Presentation (Slides)](http://slides.com/tomastrajan/angular-material-themes-guide#/)
  * [Live coding Video Tutorial](https://www.youtube.com/watch?v=PsgZjFTAleI)
  * [Meetup Presentation & Live coding Video](https://www.youtube.com/watch?v=7auj9RfCNrE)

 
## Features

* custom themes support (3 themes included)
* lazy-loading of feature modules
* lazy reducers
* localStorage ui state persistence
* `@Action Handlers` for API requests
* fully responsive design
* angular-material and custom components in `SharedModule`
 
## Stack

* Angular
* ngxs ([ngrx](https://github.com/ngrx/store) for more mature state manager or try [ngx-model](https://github.com/tomastrajan/ngx-model) if you prefer less boilerplate)
* Angular Material
* Bootstrap 4 (only reset, utils and grids)

## Troubleshooting

* **Blocking at emitting LicenseWebpackPlugin when npm start** - try using [cnpm](https://github.com/cnpm/cnpm) instead of npm

## Contributors
Want to start contributing to open source with Angular? 

Leave your mark and join the growing team of contributors!

Get started by checking out list of open [issues](https://github.com/Zuiago/angular-ngxs-material-starter/issues) and reading [Contributor Guide](https://github.com/Zuiago/angular-ngxs-material-starter/blob/master/CONTRIBUTING.md)

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<!--| [<img src="https://avatars0.githubusercontent.com/u/8050831?s=460&v=4" width="100px;"/><br /><sub><b>Iago Andrade</b></sub>](https://medium.com/@iagoquest)<br />💻 📖 ⚠ 🎨 📝 |  |  |  |  |  |  |-->
<!--| :---: | :---: | :---: | :---: | :---: | :---: | :---: |-->
<!--|  |  |  |  |-->
| [<img src="https://avatars0.githubusercontent.com/u/8050831?s=460&v=4" width="100px;"/><br /><sub><b>Iago Andrade</b></sub>](https://medium.com/@iagoquest)<br />💻 📖 ⚠ 🎨 📝 |
| :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->
