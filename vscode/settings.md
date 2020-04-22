# VS Code Settings

> update 2020-04-22（VS Code v1.44）

## Extensions

- bracket-pair-colorizer v1.0.61
- code-settings-sync v3.4.3
- EditorConfig v0.14.5
- gitlens v10.2.1
- JavaScriptSnippets v1.8.0
- material-icon-theme v4.0.1
- npm-intellisense v1.3.0
- path-intellisense v1.4.2
- prettier-vscode v4.4.0
- theme-dracula v2.21.0
- vetur v0.24.0
- vscode-ant-design-vue-helper v1.0.6
- vscode-eslint v2.1.5
- vscode-language-pack-zh-hans v1.44.2
- vuehelper v0.1.0

## Settings.json

```js
{
    "editor.quickSuggestions": {
        "strings": true
    },
    "workbench.iconTheme": "material-icon-theme",
    "git.confirmSync": false,
    "git.enableSmartCommit": true,
    "window.zoomLevel": 1,
    "sync.gist": "ec251e8ca2a58ad8341f484c464e6532",
    "sync.forceDownload": true,
    "workbench.colorTheme": "Dracula",
    // 设置保存时格式化。用于格式化html和css程序
    "editor.formatOnSave": true,
    // 关闭js/ts的默认format,统一用eslint进行格式化（tslint已经不维护了，所以转eslint吧）
    "javascript.format.enable": false,
    "typescript.format.enable": false,
    // 关闭vetur部分formatter。html用eslint-plugin-vue格式化。
    "vetur.format.defaultFormatter.html": "none",
    // js/ts程序用eslint，防止vetur中的prettier与eslint格式化冲突
    "vetur.format.defaultFormatter.js": "none",
    "vetur.format.defaultFormatter.ts": "none",
    // 设置编辑器tab宽度，用于html和css的缩近。
    "editor.tabSize": 2,
    // 开启eslint自动修复js/ts功能
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    },
    // 末尾加逗号，默认是 es5
    "prettier.trailingComma": "none"
}
```

## Extra Settings

### Settings Sync

- `Shift + Option + U` 上传；`Shift + Option + D` 下载。
- 在 `设置` 中把「Sync:Force Download」选项选上。
