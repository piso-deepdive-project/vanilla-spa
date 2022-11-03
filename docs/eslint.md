# ESLINT 설정 BY 공식문서

## Installation 설치

```shell
npm init @eslint/config
```

- How would you like to use ESLint? 강제로 스타일 적용하는지 문법만 확인할 것인지
- What type of modules does your project use? · esm cjs? mjs?
- Which framework does your project use? · react vue 어떤 프레임워크를 사용하나요
- Does your project use TypeScript? · No / Yes
- Where does your code run? · browser 노드 환경? 브라우저 환경?
- How would you like to define a style for your project? · guide
- Which style guide do you want to follow? · airbnb
- What format do you want your config file to be in? · JSON  
  Checconfig that you've selected requires the following dependencies:

### eslint-config-airbnb-base@latest eslint@^7.32.0 || ^8.2.0 eslint-plugin-import@^2.25.2

- Would you like to install them now? · No / Yes
- Which package manager do you want to use? · npm

### eslint.json이 root에 생성됩니다.

```json
{
  "env": {
    "browser": true,
    "es2021": true
  },
  "extends": "airbnb-base",
  "overrides": [],
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  "rules": {}
}
```

## eslintrc.json

### extends

#### air bnb

#### prettier

- prettier가 프로젝트 내부에서 동작할 수 있도록 설정(확장)한다

### rules

#### linebreak-style: ["error", "windows"]

- 기본 값은 "windows"가 아니라 "unix"이다. 만약 본인이 유닉스 기반의 기기라면 이 룰을 지우거나 "unix"로 수정하면 된다.

#### "quotes": ["error", "single"]

- single quote 가 아니라면 에러

#### "import/no-extraneous-dependencies": [0, { "devDependencies": ["lodash"] }]

- lodash는 devDependencies여도 에러를 띄우지말아줘
