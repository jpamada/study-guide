#### Setup and Configuration

**Install Prettier**
```sh
npm install --save-dev prettier
```

**Create File `.prettierrc`**
```json
{
  "semi": true,
  "singleQuote": true,
  "tabWidth": 2,
  "useTabs": false,
  "trailingComma": "all"
}
```

**Update `settings.json`**
```json
"editor.defaultFormatter": "esbenp.prettier-vscode",
"editor.formatOnSave": true,
"editor.insertSpaces": true,
"editor.tabSize": 2,
```

**Add Script to `package.json`**
```
{
  "scripts": {
    "format": "prettier --write ."
  }
}
```

___
#### Scripts

**Automatic Format**
```
npm run format
```