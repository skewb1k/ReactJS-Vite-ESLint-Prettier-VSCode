# ReactJS-Vite-ESLint-Prettier-VSCode

Quick setup ESLint + Prettier extintions for VSCode usefull for ReactJS + Vite

## Set up

### 1. Install extintions

```bash
code --install-extension dbaeumer.vscode-eslint
code --install-extension esbenp.prettier-vscode
code --install-extension rvest.vs-code-prettier-eslint
```

### 2. Configure your project to use it

Add `.eslintrc`, `.prettierrc`, `package.json` files in root folder of your project.

### 3. Configure VSCode settings

Open `settings.json` and add these lines to the end of file:

```json
{
  "editor.formatOnSave": true,
  "editor.formatOnPaste": false,
  "eslint.run": "onSave",
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsx]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```

## Now you can format your .js files with a simple ctrl+s
