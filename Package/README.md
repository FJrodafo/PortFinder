# PortFinder

Fast and minimalist port finder!

![NPM Collaborators](https://img.shields.io/npm/collaborators/@fjrodafo/port-finder)
![NPM Downloads](https://img.shields.io/npm/d18m/@fjrodafo/port-finder)
![NPM License](https://img.shields.io/npm/l/@fjrodafo/port-finder)
![NPM Version](https://img.shields.io/npm/v/@fjrodafo/port-finder)
![NPM Last Update](https://img.shields.io/npm/last-update/@fjrodafo/port-finder)
![NPM Unpacked Size](https://img.shields.io/npm/unpacked-size/@fjrodafo/port-finder)

## Index

1. [Install it!](#install-it)
2. [Run it!](#run-it)
3. [Environment variable](#environment-variable)
4. [Additional information](#additional-information)

## Install it!

```shell
npm i @fjrodafo/port-finder
```

## Run it!

```js
// Import the module
const { findAvailablePort } = require('@fjrodafo/port-finder');
```

```js
// It will find an available port in case port 3000 is busy
findAvailablePort(3000).then(port => {
    server.listen(port, () => {
        console.log(`Server listening on port http://localhost:${port}`);
    });
});
```

## Environment variable

```js
// You can create an environment variable for advanced use
const desiredPort = process.env.PORT ?? 3000;

findAvailablePort(desiredPort).then(port => {
    server.listen(port, () => {
        console.log(`Server listening on port http://localhost:${port}`);
    });
});
```

## Additional information

Contribute to the repository on [GitHub](https://github.com/FJrodafo/PortFinder).

Check out this package on [GitHub Packages](https://github.com/FJrodafo/PortFinder/pkgs/npm/port-finder) or [npmjs](https://www.npmjs.com/package/@fjrodafo/port-finder).