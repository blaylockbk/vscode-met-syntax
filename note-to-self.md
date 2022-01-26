# 📝 Note to self

Dear Brian,

Here are some notes about modifying and publishing this extension. Hopefully these notes help you remember what you should do.

## Developing this extension
1. Uninstall the MET syntax extension from the market place.
2. cd into your .vscode/extensions folder and git-clone the repository.

```
cd path/to/.vscode/extensions
git clone https://github.com/blaylockbk/vscode-met-syntax.git
```

3. Open the `vscode-met-syntax` folder in vscode.
4. Make some changes and then run the `Debug: Restart` command to see how the changes work (in the new window that pops open, open a sample config file)

Remember to update the `CHANGELOG.md` file with any updates to the new version.


## Update the package on marketplace

install vsce (I did this using conda in a new environment with npm installed, or just install vsce in the base environment)

```bash
conda install -c conda-forge nodejs

npm install -g vsce

cd path/to/.vscode/extensions/vscode-met-syntax
vsce package

# Here are some examples on incrementing the package version number. This command edits the `package.json` file
vsce package patch   # to increment the version by 0.0.1
vsce package minor   # to increment the version by 0.1.0
vsce package major   # to increment the version by 1.0.0

vsce publish
```

You will need a personal access token.
https://code.visualstudio.com/api/working-with-extensions/publishing-extension#get-a-personal-access-token

_Do I really have to get a new personal access token every time?_ Yes, the personal access token expires.

* sign into Azure DevOps: https://dev.azure.com/BlueLakeOrchard/
* go to create new token: https://dev.azure.com/BlueLakeOrchard/_usersSettings/tokens
* follow directions here: https://code.visualstudio.com/api/working-with-extensions/publishing-extension#get-a-personal-access-token
* note, my publisher name is `brian-blaylock`

Once you publish the extension in the marketplace, it should show here in a few minutes:
https://marketplace.visualstudio.com/items?itemName=brian-blaylock.met-syntax

**Hub URL:**
https://marketplace.visualstudio.com/manage/publishers/brian-blaylock/extensions/met-syntax/hub


**Manage the extension:**
https://marketplace.visualstudio.com/manage/publishers/brian-blaylock


# MET logo colors
- Black
- Orange #f58224


## Writing grammer

https://www.apeth.com/nonblog/stories/textmatebundle.html

https://macromates.com/manual/en/language_grammars


### Regex
* https://macromates.com/manual/en/regular_expressions
* https://regex101.com/

