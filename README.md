<div align=center>
<img src="https://github.com/blaylockbk/vscode-MET-Config/blob/main/images/met_config_logo.png?raw=true" width=200px>

<!--Badges-->
<a href="https://github.com/blaylockbk/vscode-met-config/issues"><img src="https://img.shields.io/github/issues/blaylockbk/vscode-met-config?color=blue"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=brian-blaylock.met-config"><img src="https://img.shields.io/visual-studio-marketplace/v/brian-blaylock.met-config"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=brian-blaylock.met-config"><img src="https://img.shields.io/visual-studio-marketplace/d/brian-blaylock.met-config?label=VS%20Code%20Marketplace%20Downloads"></a>
</div>

> My first ever VS Code extension 😁 inspired by [vscode-cylc](https://github.com/cylc/vscode-cylc), [mplstyle](https://github.com/yy0931/vscode-mplstyle), and [magic-python](https://github.com/MagicStack/MagicPython). This is not an extension developed by [DTC](https://dtcenter.org/community-code/model-evaluation-tools-met). I'm just a MET user.

# About

MET Config is a VS Code extension for basic syntax highlighting for Model Evaluation Tools (MET) [configuration files](https://met.readthedocs.io/en/latest/Users_Guide/config_options.html).

As an alternative, you could just use the [C/C++ Themes](https://github.com/Microsoft/vscode-cpptools) because the syntax is similar enough.

<img src="https://github.com/blaylockbk/vscode-MET-Config/blob/main/images/screenshots.png?raw=true" width=400>

- Will highlight files that have the extension `.metconfig`
- Will highlight files with the following names:

```
"filenamePatterns": [
          "PointStatConfig*",
          "GridStatConfig*",
          "EnsembleStatConfig*",
          "MODEAnalysisConfig*",
          "PB2NCConfig*",
          "STATAnalysisConfig*",
          "WaveletStatConfig*"
        ],
```

- vscode can autodect the language in a file (wonder how good this works??)
- You can manually set the file association in the settings

```json
"files.associations": {
    "PointStatConfig.txt": "met-config",
    "GridStatConfig.txt": "met-config",
}
```

## Install

Until I figure out how to publish this on the VS Code marketplace, you should just clone this repository and put the folder into your `.vscode/extensions` folder.

<br><br><br><br><br>

## Features

Describe specific features of your extension including screenshots of your extension in action. Image paths are relative to this README file.

For example if there is an image subfolder under your extension project workspace:

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

- `myExtension.enable`: enable/disable this extension
- `myExtension.thing`: set to `blah` to do something

## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension.

## Release Notes

Users appreciate release notes as you update your extension.

### 1.0.0

Initial release of ...

### 1.0.1

Fixed issue #.

### 1.1.0

Added features X, Y, and Z.

---

## Working with Markdown

**Note:** You can author your README using Visual Studio Code. Here are some useful editor keyboard shortcuts:

- Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
- Toggle preview (`Shift+CMD+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
- Press `Ctrl+Space` (Windows, Linux) or `Cmd+Space` (macOS) to see a list of Markdown snippets

### For more information

- [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
- [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**
