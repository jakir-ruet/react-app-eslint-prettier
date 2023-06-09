[![Youtube][youtube-shield]][youtube-url]
[![Facebook-Page][facebook-shield]][facebook-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<h3 align="center">
   Visit Us <a href="http://www.sunitlimitrd.com">Sun IT Limited</a>
</h3>

### React, React-TypeScript Through Eslint-Prettier Configuration

## Create App

```sh
yarn create react-app react-app-eslint --template typescript
```

## Packages & Plugin Install

Only five packages needed here no other packages is needed. It do very well, increase your productivity and increase your accuracy as well.

Checking the dependency

```sh
npm ls eslint
```

If it is not available the we Install

```sh
yarn add -D eslint
```

Or

```sh
npm i eslint --save-dev
```

Checking the dependency

```sh
npm ls eslint-plugin-typescript
```

If it is not available the we Install

```sh
yarn add -D eslint-plugin-typescript
```

Or

```sh
npm i eslint-plugin-typescript --save-dev
```

Checking the dependency

```sh
npm ls eslint-plugin-react-hooks
```

If it is not available the we Install

```sh
yarn add -D eslint-plugin-react-hooks
```

Create **.eslintrc.json** file in root directory and paste the following code block that has been cut down from **package.json** file. And we must delete the **eslintConfig** block from **package.json**.

```json
{
  "extends": ["react-app", "react-app/jest", "prettier"],
  "rules": {
    "semi": "warn"
  }
}
```

**If we need any more package/rules then will do add into the above section**

Checking the dependency

```sh
npm ls prettier
```

If it is not available the we Install

```sh
yarn add -D prettier
```

Checking the dependency

```sh
npm ls eslint-config-prettier
```

If it is not available the we Install

```sh
yarn add -D eslint-config-prettier
```

Create **.prettierrc.json** and paste/type the following code block.

```json
{
  "singleQuote": true
}
```

**If we need others rules of prettier. We can add the above section as per requirement.**

Create **.prettierignore** and paste the following lines & we can add/remove as per the requirement.

```sh
/build
/node_modules
/package-lock.json
/yarn-error.log
/yarn.lock
```

Create **settings.json** into **.vscode** directory and paste the following lines & we can add/remove as per the requirement.

```sh
{
  // Eslint-Prettier Section
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "[html]": {
    "editor.formatOnSave": true
  },
  "[javascript]": {
    "editor.formatOnSave": false
  },
  "[javascriptreact]": {
    "editor.formatOnSave": false
  },
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "eslint.alwaysShowStatus": true,
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact"
  ],
  // Prettier Section
  "prettier.tabWidth": 2,
  "prettier.useTabs": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "avoid",
  "prettier.jsxSingleQuote": false
}
```

For applying the prettier we just use these command on terminal, then it work.

```sh
yarn prettier --write .
```

Then

```sh
npx prettier --check .
```

## VS Code Chrome Debugger Extension install & configuration.

We just create **launch.json** into the **.vscode** and paste the following code block.

```sh
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Chrome",
      "type": "chrome",
      "request": "launch",
      "url": "http://localhost:3000",
      "webRoot": "${workspaceFolder}/src",
      "sourceMapPathOverrides": {
        "webpack:///src/*": "${webRoot}/*"
      }
    }
  ]
}
```

## Courtesy of Jakir,

<a href="https://www.linkedin.com/in/jakir-ruet/">LinkedIn</a>
<a href="https://www.facebook.com/jakir.ruet">Facebook</a>
<a href="https://github.com/jakir-ruet">GitHub</a>
<a href="https://web.skype.com/?openPstnPage=true">Skype</a>

## Have good day, stay with me.

[youtube-shield]: https://img.shields.io/badge/-Youtube-black.svg?style=flat-square&logo=youtube&color=blue&logoColor=red
[youtube-url]: https://www.youtube.com/watch?v=9i424dXt2Pk
[facebook-shield]: https://img.shields.io/badge/-Facebook-black.svg?style=flat-square&logo=facebook&color=pink&logoColor=blue
[facebook-url]: https://www.facebook.com/SunItLimited/
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=red
[linkedin-url]: https://www.linkedin.com/company/gosunitlimited
