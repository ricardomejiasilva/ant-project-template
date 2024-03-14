## React project with Typescript Less and Vite
 This project template is set up with React, Vite, TypeScript, and Less CSS, providing a robust starting point for building modern web applications with strong type-checking and customizable styles.

## Prerequisites
Before you begin, ensure you have the following installed:
  Node.js (LTS version recommended)
  npm or Yarn


## Installation
Start the development server:

```sh
npm install
```

## Run the project
This command will launch the project in your default web browser. You should see the app running at with the local link on your terminal

```sh
npm run dev
```

## Usage
After starting the development server, you can begin to develop your application. The project is already set up to use React for UI components, TypeScript for static type checking, and Less for styling.


## Build
This command will launch the project in your default web browser. You should see the app running at http://localhost:3000.

```sh
npm run build
```

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
