Dear Brian,

To update the package, please run:

install vsce ( I just did this in the base environment)

```
conda install -c conda-forge nodejs

npm install -g vsce

cd myExtension
vsce package

vsce package patch   # to increment the version by 0.0.1
vsce package minor   # to increment the version by 0.1.0
vsce package major   # to increment the version by 1.0.0

vsce publish
```

You will need a personal access token.
https://code.visualstudio.com/api/working-with-extensions/publishing-extension#get-a-personal-access-token

( Do I really have to do that every time? ) 

It should show here in a few minutes:
https://marketplace.visualstudio.com/items?itemName=brian-blaylock.metconfig