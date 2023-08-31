<p align="center">
    <img width="400" src="https://github.com/ArcherGu/fast-vite-electron/blob/main/logo.png" alt="logo">
</p>

# ⚡Vite + Electron & Doubleshot Template

This template is used to build vite + electron projects. Build with [Doubleshot](https://github.com/Doubleshotjs/doubleshot), crazy fast!

🎉 [Doubleshot](https://github.com/Doubleshotjs/doubleshot) is a whole new set of tools to help you quickly build and start a node backend or electron main process.

## Features

- 🔨 [vite-plugin-doubleshot](https://github.com/archergu/doubleshot/tree/main/packages/plugin-vite#readme) to run/build electron main process.
<br>

- 😎 Controllers/Services ipc communication, powered by Typescript [decorators](https://www.typescriptlang.org/docs/handbook/decorators.html).
<br>

- ⚡ Rendering process is powered by [Vite](https://vite.io/).
<br>

- ⏩ Quick start and build, powered by [tsup](https://tsup.egoist.sh/) and [electron-builder](https://www.electron.build/) integrated in [@doubleshot/builder](https://github.com/Doubleshotjs/doubleshot/tree/main/packages/builder)

## Motivation

In the past, I've been building desktop clients with [vue](https://v3.vuejs.org/) + [vue-cli-plugin-electron-builder](https://github.com/nklayman/vue-cli-plugin-electron-builder), and they work very well. But as the project volume grows, webpack-based build patterns become slower and slower.

The advent of [vite](https://vitejs.dev/) and [esbuild](https://esbuild.github.io/) greatly improved the development experience and made me feel lightning fast ⚡.

 It took me a little time to extract this template and thank you for using it.

## How to use

- Click the [Use this template](https://github.com/ArcherGu/fast-vite-electron/generate) button (you must be logged in) or just clone this repo.
- In the project folder: 
  ```bash
  # install dependencies
  yarn # npm install

  # run in developer mode
  yarn dev # npm run dev

  # build
  yarn build # npm run build
  ```

## Note for PNPM

In order to use with `pnpm`, you'll need to adjust your `.npmrc` to use any one the following approaches in order for your dependencies to be bundled correctly (ref: [#6389](https://github.com/electron-userland/electron-builder/issues/6289#issuecomment-1042620422)):
```
node-linker=hoisted
```
```
public-hoist-pattern=*
```
```
shamefully-hoist=true
```

