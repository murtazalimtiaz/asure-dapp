## Quick Overview

```sh
# We require a recent version of  npm.
npm install -g npm

# NOTE: Only for Windows users.
# All our npm scripts expect to be run in a
# sh shell. On Windows we use the npm config option
# `script-shell` and point it to the Git Bash shell.
# This config option can be set globally or per npm
# package by using an .npmrc file.
# We prepared a little script that creates an .npmrc
# file in each npm package and sets script-shell to
# `C:\Program Files\Git\bin\bash.exe`. It also adds
# `C:\Program Files\Git\bin` to your PATH variable.

#### call tools/init-win.cmd

# Install dependencies.
npm install

# Start Ganache. Ganache will deploy all smart
# contracts and test data.  This will take a
# few minutes.
npm run start-smartcontracts

# Start the dapp.
npm run start-dapp