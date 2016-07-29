# Skeleton

Jump-start your front-end development. Skeleton is a HTML5 Boilerplate build upon [Rosid](https://github.com/electerious/Rosid).

## Contents

- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [How to use](#how-to-use)
	- [Develop](#develop)
	- [Compile](#compile)

## Features

- Skeleton is a base for all your everyday web-projects. Jump-start your work and develop without starting from zero. Everything you need one fork away.
- This project is powered by [Rosid](https://github.com/electerious/Rosid), a web server with just-in-time pre-processing. JS (with Babel, UglifyJS), SASS (with cssnano, Autoprefixer) and EJS can be used right out of the box.
- Skeleton is just the beginning. Fork it and extend it to your own needs. The predefined structure gives you flexibility and can be modified with ease.

## Requirements

Skeleton dependents on …

- [Node.js](https://nodejs.org/en/) (v6.2.0 or newer)
- [npm](https://www.npmjs.com)
- [Bower](http://bower.io)

Make sure to install and update all dependencies before you fork and setup Skeleton.

## Setup

We recommend to download Skeleton from GitHub using git:

```sh
git clone https://github.com/electerious/Skeleton
```

Install all required dependencies from both [npm](https://www.npmjs.com) and [Bower](http://bower.io) before you start with the development. All steps are combined into one single command, which can be executed when both package managers are installed on your system.

```sh
npm install
```

## How to use

### Develop

Start developing using the following command. You browser will open, wait for code-changes and live-reload instantly when you update your files. JS, SASS and EJS will be compiled on-the-fly.

```sh
npm start
```

### Compile

Ready for prime time? Export all files, compiled and prepared for your audience. Simple upload the final `dist/` folder to your server and relax. Take a seat and enjoy a delicious burger from your favorite restaurant.

```sh
npm run compile
```

## Docker

The included Dockerfile lets you build an image which compiles your site. In this case only Docker needs to be installed on the system. No other dependencies are required.

### Build

Build an image from the Dockerfile. This has to be done each time you have modified the project. The new source will be copied into the image.

```sh
docker build -t electerious/skeleton .
```

### Compile

Start a container to compile your site. The container will exit automatically when all tasks have been finished. The mounted volume will contain all compiled files.


```sh
docker run --rm -t -v $(pwd)/dist:/dist electerious/skeleton
```