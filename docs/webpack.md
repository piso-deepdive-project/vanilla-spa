# Webpack

## Installation 설치

### Basic Install 기본 설치

```shell
npm i -D webpack webpack-cli
```

- package.json `"main": "index.js"` 를 삭제하고 `"private": true`를 추가한다.
- 왜냐하면 접근을 막기위해서

```shell
npm i -D lodash
```

- lodash 라이브러리를 설치해주는데, 이유는 index.js안에 사용된 문법이 lodash 문법(\_)이기 때문이다.

## Configuration 환경설정

- 원래 4 버전부터 필요없는데, 기존의 프로젝트들의 파일을 위해 존재한다. - `webpack.config.js`

```javascript
const path = require("path");

module.exports = {
  entry: "./src/index.js", // 파일을 묶을 입구
  output: {
    filename: "main.js", // 결과물 이름
    path: path.resolve(__dirname, "dist"), // 생성될 폴더
  },
};
```
