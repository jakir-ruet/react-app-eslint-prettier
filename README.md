[![Youtube][youtube-shield]][youtube-url]
[![Facebook-Page][facebook-shield]][facebook-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<h3 align="center">
   Visit Us <a href="http://www.sunitlimitrd.com">Sun IT Limited</a>
</h3>

### React, React-TypeScript Through Eslint-Prettier Configuration

<h4>Create ReactJS/ReactJS-TypeScript App</h4>
-[Create App](#Create-App)

<h4>Only Five Packages Needed</h4>
-[Eslint](#ddddd)
-[Eslint Plugin React/TypeScript](#ddddd)
-[Eslint Plugin React Hooks](#ddddd)
-[Prettier](#ddddd)
-[Eslint Config Prettier](#ddddd)

## Create App

```sh
yarn create react-app react-app-eslint --template typescript
```

yarn create react-app react-app-eslint --template typescript

Checking the dependency then install

npm ls eslint
yarn add -D eslint
Or
npm i eslint --save-dev

npm ls eslint-plugin-typescript
yarn add -D eslint-plugin-typescript
Or
npm i eslint-plugin-typescript --save-dev

Create .eslintrc.json and paste
"extends": ["react-app", "react-app/jest", "prettier"],
"rules": {
"semi": "warn"
}

npm ls eslint-plugin-react-hooks
yarn add -D eslint-plugin-react-hooks

npm ls prettier
yarn add -D prettier

npm ls eslint-config-prettier
yarn add -D eslint-config-prettier

Create .prettierrc.json and paste
{
"singleQuote": true
}

Create .prettierignore and paste
/build
/node_modules
/package-lock.json
/yarn-error.log
/yarn.lock

yarn prettier --write .
npx prettier --check .

[youtube-shield]: https://img.shields.io/badge/-Youtube-black.svg?style=flat-square&logo=youtube&color=blue&logoColor=red
[youtube-url]: https://www.youtube.com/watch?v=9i424dXt2Pk
[facebook-shield]: https://img.shields.io/badge/-Facebook-black.svg?style=flat-square&logo=facebook&color=pink&logoColor=blue
[facebook-url]: https://www.facebook.com/SunItLimited/
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=red
[linkedin-url]: https://www.linkedin.com/company/gosunitlimited
