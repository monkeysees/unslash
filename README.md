<h1 align="center">Unslash</h1>

<div align="center">
   Solution for a challenge from  <a href="http://devchallenges.io" 
target="_blank">Devchallenges.io</a>.
</div>

<div align="center">
  <h3>
    <!-- <a href="https://unslash.islambeg.me/">
      Demo
    </a>
    <span> | </span>
    <a 
href="https://gitlab.com/islambeg-frontend-projects/fullstack/unslash/README">
      Solution
    </a>
    <span> | </span>
    <a href="https://devchallenges.io/challenges/O2iGT9yBd6xZBrOcVirx">
      Challenge (part 1)
    </a>
    /
    <a href="https://devchallenges.io/challenges/rYyhwJAxMfES5jNQ9YsP">
      Challenge (part 2)
    </a> -->
  </h3>
</div>

## Table of Contents

- [Overview](#overview)
  - [Built With](#built-with)
- [Features](#features)
- [How to use](#how-to-use)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Overview

This is a fullstack app which features a private image repository inspired 
by [Unsplash](https://unsplash.com/).

It is built with Express on the server side and Vue 3 on the frontend, 
using Typescript on both ends. Uploaded files are stored on server's 
filesystem with info about them saved to LevelDB.

<!-- - [Client 
repository](https://gitlab.com/islambeg-frontend-projects/fullstack/unslash/client)
- [Server 
repository](https://gitlab.com/islambeg-frontend-projects/fullstack/unslash/server) -->

Building this app helped me to better understand how file uploading works 
as well as get a glimpse of what fullstack development process looks like.

### Built With

- [Express](https://expressjs.com/)
- [LevelDB](https://github.com/google/leveldb)
- [Vue.js](https://vuejs.org/)
- [Pinia](https://pinia.vuejs.org/)
- [Typescript](https://www.typescriptlang.org/)
- [Sass](https://sass-lang.com/)
- [Vite](vitejs.dev/)

## Features

- Add your images by uploading them or providing URL
- Delete unwanted images
- Search uploaded images by label

Please be aware that app is currently hosted for demonstration purposes 
only. This means that there are certain limitations:
1) images upload size is limited by 15 MB
2) session lifespan is limited by 2 days after which user data will be 
restored to the initial state, i.e., all uploaded images will be deleted.

If you wish to hos the app yourself these settings can be customized by 
setting appropriate environment variables.

## How To Use

To clone and run this application on your local machine, you'll need 
[Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) 
(which comes with [npm](http://npmjs.com)) installed on your computer. 
Keep in mind that environment variables have to be provided in 
`.env.development.local` (see `.env.example`) for both client and server.

From your command line:

```bash
# Create main directory for project and enter it
$ mkdir unslash && cd unslash

# Clone client & server repositories
# $ git clone 
# https://gitlab.com/islambeg-frontend-projects/fullstack/unslash/client && 
# git clone 
# https://gitlab.com/islambeg-frontend-projects/fullstack/unslash/server

# Install client & server dependencies
$ npm --prefix ./client install && npm --prefix ./server install

# Start server in dev mode
$ npm --prefix ./server run dev

# Start client in dev mode
$ npm --prefix ./client run dev
```

## Acknowledgements

- [TypeScript Express tutorial by Marcin 
Wanago](https://wanago.io/courses/typescript-express-tutorial/)
- [How To Make A Drag-and-Drop File Uploader With Vue.js 3 by Joseph 
Zimmerman](https://www.smashingmagazine.com/2022/03/drag-drop-file-uploader-vuejs-3/)
- [How to Favicon in 2022 by Andrey 
Sitnik](https://evilmartians.com/chronicles/how-to-favicon-in-2021-six-files-that-fit-most-needs)
- [Using JavaScript to trap focus in an element by Hidde de 
Vries](https://hidde.blog/-using-javascript-to-trap-focus-in-an-element/)
- [Load all focusable elements with JavaScript by Andy 
Bell](https://piccalil.li/quick-tip/load-all-focusable-elements-with-javascript/)
- [Infinite CSS Loading Spinner by Taha 
Aijjou](https://codepen.io/taha-aijjou/pen/dKvjxJ)

## Contact

- Email monkeyseesone@gmail.com
