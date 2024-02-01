[![LinkedIn][linkedin-shield-lapissoft]][linkedin-url-lapissoft]
[![Facebook-Page][facebook-shield-lapissoft]][facebook-url-lapissoft]
[![Youtube][youtube-shield-lapissoft]][youtube-url-lapissoft]

## Visit Us [Lapis Soft](http://www.lapissoft.com)

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

## Courtesy of Jakir

[![LinkedIn][linkedin-shield-jakir]][linkedin-url-jakir]
[![Facebook-Page][facebook-shield-jakir]][facebook-url-jakir]
[![Youtube][youtube-shield-jakir]][youtube-url-jakir]

### Have a good day, stay with me
<!-- Personal profile -->

[linkedin-shield-jakir]: https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url-jakir]: https://www.linkedin.com/in/jakir-ruet/
[facebook-shield-jakir]: https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white
[facebook-url-jakir]: https://www.facebook.com/jakir-ruet/
[youtube-shield-jakir]: https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white
[youtube-url-jakir]: https://www.youtube.com/@mjakaria-ruet/featured

<!-- Company profile -->

[linkedin-shield-lapissoft]: https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white
[linkedin-url-lapissoft]: https://www.linkedin.com/company/lapis-soft/
[facebook-shield-lapissoft]: https://img.shields.io/badge/Facebook-%231877F2.svg?style=for-the-badge&logo=Facebook&logoColor=white
[facebook-url-lapissoft]: https://www.facebook.com/GoLapisSoft/
[youtube-shield-lapissoft]: https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white
[youtube-url-lapissoft]: https://www.youtube.com/@LapisSoft/featured
