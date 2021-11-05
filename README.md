<div align=center>
<img src="https://github.com/blaylockbk/vscode-metconfig/blob/main/images/metconfig_logo_white.png?raw=true" width=250px>

<!--Badges-->

<a href="https://github.com/blaylockbk/vscode-metconfig/issues"><img src="https://img.shields.io/github/issues/blaylockbk/vscode-metconfig?color=blue"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=brian-blaylock.metconfig"><img src="https://img.shields.io/visual-studio-marketplace/v/brian-blaylock.metconfig"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=brian-blaylock.metconfig"><img src="https://img.shields.io/visual-studio-marketplace/d/brian-blaylock.metconfig"></a>

<!--(end badges)-->
</div>

> My first ever VS Code extension 😁 inspired by [vscode-cylc](https://github.com/cylc/vscode-cylc), [mplstyle](https://github.com/yy0931/vscode-mplstyle), and [magic-python](https://github.com/MagicStack/MagicPython).  
> This is not an extension developed by [DTC](https://dtcenter.org/community-code/model-evaluation-tools-met). I'm just a MET user.

# About

"MET config" is a VS Code extension for basic syntax highlighting for [Model Evaluation Tools](https://dtcenter.org/community-code/model-evaluation-tools-met) (MET) [configuration files](https://met.readthedocs.io/en/latest/Users_Guide/config_options.html).

This extension looks best with dark themes in VS Code for now.

It highlights the following:

- comments
- strings
- environment variables (i.e., `${ENV_VAR}`)
- numbers
- keywords (TRUE, FALSE, NONE, UNION, NA, SQUARE, etc.)

<img src="https://github.com/blaylockbk/vscode-MET-Config/blob/main/images/screenshots.png?raw=true">

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
    "PointStatConfig.txt": "metconfig",
    "GridStatConfig.txt": "metconfig",
}
```

## Install

Install from the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=brian-blaylock.metconfig).

Or, you can clone this repository and put the folder into your `~/.vscode/extensions` folder.

## Alternatives?

The only alternative that produces anything similar (that I have found) is setting the code format to C/C++ because the syntax is similar enough, but this mississ highlighting MET-specific keywords and environment variables.

**Enjoy!**
