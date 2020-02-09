# VS Code Settings

> update 2020-02-08（VS Code v1.42）

## Extensions

*   bracket-pair-colorizer v1.0.61
*   code-settings-sync v3.4.3
*   gitlens v10.2.0
*   material-icon-theme v3.9.2
*   path-intellisense v1.4.2
*   svn-scm v2.6.1
*   theme-dracula v2.19.2
*   vetur v0.23.0
*   vscode-ant-design-vue-helper v1.0.6
*   vscode-eslint v2.0.15
*   vscode-language-pack-zh-hans v1.42.2
*   vuehelper v0.1.0

## Settings.json

```js
{
    "editor.quickSuggestions": {
        "strings": true
    },
    "workbench.iconTheme": "material-icon-theme",
    "git.confirmSync": false,
    "git.enableSmartCommit": true,
    "window.zoomLevel": 0,
    "sync.gist": "[your gist]",
    "sync.forceDownload": true,
    "workbench.colorTheme": "Dracula",
    // 2020-02-08 https://zhuanlan.zhihu.com/p/103492877
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
    }
}
```

## Extra Settings

### Settings Sync

* `Shift + Option + U` 上传；`Shift + Option + D` 下载。
* 在 `设置` 中把「Sync:Force Download」选项选上。