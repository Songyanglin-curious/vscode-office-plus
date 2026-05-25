# Officew Viewer

## Fork notice

Office Viewer Plus is a fork of [cweijan/vscode-office](https://github.com/cweijan/vscode-office). The original Office Viewer extension, its office-file preview features, and most of the extension architecture were created by the original author and contributors.

This fork is published separately so it can update the Markdown editor engine: the bundled Vditor assets were upgraded to `vditor@3.11.2`, Mermaid was upgraded to `11.11.0`, and the Markdown editor now loads these assets from the extension package instead of a remote CDN. The goal is better local/offline Markdown editing and improved Mermaid rendering while preserving the original extension's work.

## Introduction

English | [简体中文](README-CN.md) | [繁體中文](README-TW.md)

This extension supports previewing these common office file formats in VS Code.

- Excel: .xls, .xlsx, .csv
- Word: .docx
- Svg: .svg
- Pdf: .pdf
- Font: .ttf, .otf, .woff, .woff2
- Markdown: .md
- HttpRequest: .http
- Windows Reg: .reg
- Compressed file: .zip, .jar, .vsix, .rar

## Markdown

This extension changes the default markdown editor to the vditor. **Please note that this editor is no longer actively maintained.**

If you want to use the original vscode editor, insert this in your `settings.json`.

```json
{
    "workbench.editorAssociations": {
        "*.md": "default",
        "*.markdown": "default"
    }
}
```

Shortcuts: Base on [Vditor shortcuts](shortcut.md) and more:

- Move list up: `Ctrl Alt I` / `⌘ ^ I`
- Move list down: `Ctrl Alt J` / `⌘ ^ J`
- Edit in VS Code: `Ctrl Alt E` / `⌘ ^ E`

Tips:

- Resize editor via ctrl/cmd+mouse scroll.
- Hyperlinks can be opened by ctrl/meta+click or double-click.

## HTML

The html editor supports live viewing.   Press ctrl+shift+v to open the live view.

## Sponsor

[![Database Client](https://database-client.com/text_logo.png)](https://marketplace.visualstudio.com/items?itemName=cweijan.vscode-database-client2)

Database Client for Visual Studio Code, supporting the management **MySQL/MariaDB, PostgreSQL, SQLite, Redis** and  **ElasticSearch**, and works as an **SSH** client, boost your maximum productivity! [Get it now](https://marketplace.visualstudio.com/items?itemName=cweijan.vscode-database-client2).

## Credits

- Original extension: [cweijan/vscode-office](https://github.com/cweijan/vscode-office)
- PDF rendering: [mozilla/pdf.js/](https://github.com/mozilla/pdf.js/)
- Docx rendering: [VolodymyrBaydalka/docxjs](https://github.com/VolodymyrBaydalka/docxjs)
- XLSX rendering:
  - [SheetJS/sheetjs](https://github.com/SheetJS/sheetjs): XLSX parsing
  - [myliang/x-spreadsheet](https://github.com/myliang/x-spreadsheet): XLSX rendering
- HTTP: [Rest  Client](https://github.com/Huachao/vscode-restclient)
- Markdown editor: [Vanessa219/vditor](https://github.com/Vanessa219/vditor), bundled in this fork as `vditor@3.11.2`
- Mermaid rendering: [mermaid-js/mermaid](https://github.com/mermaid-js/mermaid), bundled in this fork as Mermaid `11.11.0`
- Material Icon theme: [PKief/vscode-material-icon-theme](https://github.com/PKief/vscode-material-icon-theme)
