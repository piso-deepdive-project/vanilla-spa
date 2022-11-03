# Webpack

## Install

### Basic Install

```shell
npm i -D webpack webpack-cli
```

- package.json `"main": "index.js"` 를 삭제하고 `"private": true`를 추가한다.
- 왜냐하면 접근을 막기위해서

```shell
npm i -D lodash
```

- lodash 라이브러리를 설치해주는데, 이유는 index.js안에 사용된 문법이 lodash 문법(\_)이기 때문이다.
