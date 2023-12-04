# -template-web

前端流行项目模版，非严格自由难以控制的的项目。

## `package.json`文件依赖插件

```json
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview",
    "prepare": "husky install",
    "format": "npx prettier . --write"
  },
  "dependencies": {
    "ant-design-vue": "^4.0.7",
    "pinia": "^2.1.7",
    "vue": "^3.3.4",
    "vue-router": "^4.2.5"
  },
  "devDependencies": {
    "@vitejs/plugin-vue": "^4.4.0",
    "autoprefixer": "^10.4.16",
    "husky": "^8.0.0",
    "lint-staged": "^15.1.0",
    "postcss": "^8.4.32",
    "prettier": "3.1.0",
    "tailwindcss": "^3.3.5",
    "vite": "^4.4.11"
  }
```

## `name`、`version`、`private`相关

在`package.json`文件中除了关键的信息，还有几个字段，`name`、`version`、`private`。如果我们不开发npm包就不需要关心这些信息。
