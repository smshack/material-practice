# 1. 리액트 기초 구성
```javascript
npx create-react-app react-app
cd react-app

## 타입 스크립트 사용
yarn add typescript @types/node @types/react @types/react-dom @types/jest

## tsconfig.json 파일 추가
npx typescript --init

## 불필요한 파일 제거
yarn add scss sass
yarn add  @mui/material @emotion/react @emotion/styled

yarn add @fontsource/roboto
```

# 2. eslint 설정
```
npx eslint --init

## .eslintrc.js 생성됨
module.exports = {
    "env": {
        "browser": true,
        "commonjs": true,
        "es2021": true
    },
    "extends": [
        "eslint:recommended",
        "plugin:react/recommended",
        "plugin:@typescript-eslint/recommended"
    ],
    "overrides": [
    ],
    "parser": "@typescript-eslint/parser",
    "parserOptions": {
        "ecmaVersion": "latest"
    },
    "plugins": [
        "react",
        "@typescript-eslint"
    ],
    "rules": {
    }
}
```

# 3. prettier 설정
```
yarn add eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-prettier eslint-config-prettier


eslint-plugin-import : ES6의 import, export 구문을 지원, 필수 플러그인
eslint-plugin-react : React 규칙이 들어있는 플러그인
eslint-plugin-react-hooks : React Hooks 규칙이 들어있는 플러그인
eslint-plugin-jsx-a11y : JSX요소의 접근성 규칙에 대한 정적 검사 플러그인

root폴더에서 .prettierrc 생성
```

# 4. Typography
https://mui.com/material-ui/react-typography/