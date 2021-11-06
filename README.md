<div align=center>
<img src="https://github.com/blaylockbk/vscode-met-syntax/blob/main/images/met-syntax_logo_white.png?raw=true" width=250px>

<!--Badges-->

<a href="https://marketplace.visualstudio.com/items?itemName=brian-blaylock.met-syntax"><img src="https://img.shields.io/visual-studio-marketplace/v/brian-blaylock.met-syntax"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=brian-blaylock.met-syntax"><img src="https://img.shields.io/visual-studio-marketplace/d/brian-blaylock.met-syntax"></a>
<a href="https://github.com/blaylockbk/vscode-met-syntax"><img src="https://img.shields.io/github/stars/blaylockbk/vscode-met-syntax"></a>
<a href="https://github.com/blaylockbk/vscode-met-syntax/issues"><img src="https://img.shields.io/github/issues/blaylockbk/vscode-met-syntax?color=blue"></a>   

<!--(end badges)-->
</div>

> My first ever VS Code extension 😁 inspired by [vscode-cylc](https://github.com/cylc/vscode-cylc), [mplstyle](https://github.com/yy0931/vscode-mplstyle), and [magic-python](https://github.com/MagicStack/MagicPython).  
> This is not an extension developed by [DTC](https://dtcenter.org/community-code/model-evaluation-tools-met). I'm just a MET user.

# About

**MET syntax** is a VS Code extension for basic syntax highlighting of [Model Evaluation Tools](https://dtcenter.org/community-code/model-evaluation-tools-met) (MET) [configuration files](https://met.readthedocs.io/en/latest/Users_Guide/config_options.html).

This extension currently looks best with dark themes in VS Code.

Syntax highlighting can help you visually understand MET configuration file structure and help you catch errors. The following are highlighted:

- comments
- strings
- environment variables (i.e., `${ENV_VAR}`)
- numbers
- keywords (TRUE, FALSE, NONE, UNION, NA, SQUARE, etc.).

<img src="https://raw.githubusercontent.com/blaylockbk/vscode-met-syntax/main/images/compare.png">

Highlighting is applied to files with the extension `.metconfig` and to files with the following filename patterns:

- `*PointStatConfig*`
- `*GridStatConfig*`
- `*EnsembleStatConfig*`
- `*MODEAnalysisConfig*`
- `*PB2NCConfig*`
- `*STATAnalysisConfig*`
- `*WaveletStatConfig*`

For any other files, you should manually set the file association in your settings. For example,

```json
"files.associations": {
    "myMETConfigFile": "metconfig",
}
```

## Install

Install from the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=brian-blaylock.met-syntax).

Or, you can clone this repository into your `~/.vscode/extensions/` folder.

## Potential Improvements

This is my first VS Code extension. I threw this together quickly after watching a tutorial, but there is potential with this extension to do so much more! If you want to make improvements, your pull requests are welcomed.

- snippets
- code validation
- code completion
- highlighting for METplus wrapper files

---

**Enjoy!**

\- Brian Blaylock
