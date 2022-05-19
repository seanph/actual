# Actual

This is my personal fork of [Actual](https://actualbudget.com) (original repo [here](https://github.com/actualbudget/actual)). Actual is a free and open-source, local-first personal finance tool.

## Installation

```
git clone https://github.com/seanph/actual.git
cd actual
yarn install

# make changes to, eg. /packages/desktop-client

cd packages/desktop-client
yarn link

# back to a home directory

git clone https://github.com/actualbudget/actual-server.git
cd actual-server
yarn install
yarn start
```

Navigate to <https://localhost:5006> in your browser and you will see Actual.

## Run locally

Both the electron and web app can started with a single command. When running in development, it will store data in a `data` directory in the root of the `actual` directory.

First, make sure to run `yarn install` to install all dependencies.

In the root of the project:

```
yarn start            # Run the electron app
yarn start:browser    # Run the web app
```

## Code structure

The app is split up into a few packages:

* `loot-core`: The core application that runs on any platform
* `loot-design`: The generic design components that make up the UI
* `desktop-client`: The desktop UI
* `desktop-electron`: The desktop app
* `mobile`: The mobile app

More docs are available in the [docs](https://github.com/actualbudget/actual/tree/master/docs) folder.
