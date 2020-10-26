# DIY Wiki

 This is a fullstack project to build a mini markdown wiki web app.
This project has been developed using the _development strategy_ concept with one branch per step.
It is a way to develop a fullstack web app using node.js and react.

## Table of contents

* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## General info

- This project is a simple way to develop several skills
  - Debugging Node apps in VSC
  - Using npm: installing dependencies, running scripts
  - Understanding what "fullstack" means
  - Using branches
  - Running the Frontend & Backend separately
  - Node.js & Express Skills

- The purpose is to be familiar with node.js.
- For intermediate level.

> The start repo is: [diy-wiki repository](https://github.com/hackyourfuturebelgium/diy-wiki)

## Screenshots

![Example screenshot](public/assets/images/wireframe-diy-wiki.png)

## Technologies

* HTML5
* Javascript
* Node.js
* Express
* React
* Git & Github

## Setup

### Running the API


__Installing Dependencies__

1. `npm install`

__Running the API__

1. `npm run dev`
2. Open Postman
3. Explore `localhost:xxxx`!


### Running the Frontend

__Installing Dependencies__
<<<<<<< HEAD

1. `npm install`

__Running the Frontend__
=======
1. `npm install` || `yarn install`

__Building the Frontend__
1. `npm run build` || `yarn build`


[TOP](#do-it-yourself-wiki)

---

## Your Task

What you need to do to complete this assignment is write the 5 routes described in the `./wiki-server/server.js' file.  You'll know your work is finished when you can use every button, link, and page in your frontend!

We recommend always keeping the live demo open as you develop to be sure you keep the final product in mind.  You can find the link in a pinned message on your class' Slack channel.

### Get an Existing Page

Calling this route should return a response with a property called `body` containing the text stored inside the file with the name `:slug`

* _method_: GET
* _path_: `"/api/page/:slug"`
* _success response_: `{status: 'ok', body: '<file contents>'}`
* _failure response_: `{status: 'error', message: 'Page does not exist.'}`

### Post a New Page

Calling this route with a `body` property in the body of your HTTP Request, and a file name in the `:slug` URL parameter will add a new markdown file to the `./wiki-server/data` directory

* _method_: POST
* _path_: `"/api/page/:slug"`
* _body_: `{body: '<file content>'}`
* _success response_: `{status: 'ok'}`
* _failure response_: `{status: 'error', message: 'Could not write page.'}`


### Get All Page Names

Calling this route will return a response with a property called `pages` which is an array containing all of the file names in `./wiki-server/data`.

* _method_: GET
* _path_: `"/api/page/all"`
* _success response_: `{status:'ok', pages: ['fileName', 'otherFileName']}`
* _failure response_: (none)


### Get All tags


Calling this route will return a response with a property called `tags` which is an array containing all of the tagged words in all of the files of `./wiki-server/data`. Tagged words are any word in a file with a # in front of it, like so `#tree`.  Or `#table`,

* _method_: GET
* _path_: `"/api/tags/all"`
* _success response_: `{status:'ok', tags: ['tagName', 'otherTagName']}`
* _failure response_: (none)


### Get Page Names by Tag

Calling this route will return a response with a property called `tag` which indicates which tag was used to search, and a property called `pages` which is an array of all the file names containing that tag

* _method_: GET
* _path_: `"/api/tags/:tag"`
* _success response_: `{status:'ok', tag: 'tagName', pages: ['tagName', 'otherTagName']}`
* _failure response_: (none)


[TOP](#do-it-yourself-wiki)

---

## Helpful Links



__Debugging JS Servers In VSC__

* [VSC Debugger (from the docs)](https://code.visualstudio.com/docs/editor/debugging)
* [Debugging Node apps (from the docs)](https://code.visualstudio.com/docs/nodejs/nodejs-debugging)
* [Express in VSC (video)](https://www.youtube.com/watch?v=2oFKNL7vYV8)
* [Express in VSC (another video)](https://www.youtube.com/watch?v=yFtU6_UaOtA)

__Node.js Tutorials__

These tutorials will introduce you to a bunch of new features in Node that you haven't seen in the Browser.  While you're following these tutorials, it's important to remember that at it's core Node.js is still JavaScript.  Everything you've learned so far (except for the DOM & `fetch` :) is still true!  The Event Loop, Classes, Closure, Arrays, Objects, Variables, `this.`, it's all still the same.


The tutorials below will introduce to what's new and what's special about Node.  But don't forget to take some time and solve a few of the JavaScript Exercises above to get used to working with plain, vanilla JS in the terminal.

* [Traversy: Node for Absolute Beginners](https://www.youtube.com/watch?v=U8XF6AFGqlc)
* [Traversy: Node.js Crash Course](https://www.youtube.com/watch?v=fBNz5xF-Kx4)
* [Mosh: Node.js in 1 Hour](https://www.youtube.com/watch?v=TlB_eWDSMt4)

>>>>>>> e242be7c86b3c130255931cc546328c77758c55d

1. `npm run start`
2. It will automatically open a new tab in your browser
3. Explore the wiki API from the frontend app!

## Code Examples

Examples of usage:

   `to be added later`


## Features

List of features :

* Asynchronous
* Applying Incremental Development 
* Single threaded

To-do list:

*Add search engin

## Status

Project is: _in progress_

## Inspiration

Project inspired by HYF

## Contact

Routes part Created by [@eltayeb](https://github.com/Eltayeb-Elgaali) - feel free to contact me!