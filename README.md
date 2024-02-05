# VS Code Cheat Sheet
VS Code Cheat Sheet with the most needed stuff..






<br><br>







# Install
- https://code.visualstudio.com/Download
  - You should not install it via snap because then it is read only and the code from below at extensions will not work


<br><br>






# Update

## Linux
- Check if you installed VS Code via debian file or via snap store
```shell
#.deb
dpkg -l | grep code

# snap
snap list code
```
- If you installed via .deb just download the latest one and then install it
  ```shell
  sudo apt install xxx.deb
  ```



<br><br>
______________________________________________________
______________________________________________________
<br><br>




# Uninstall 

<br><br>

## Fedora
```
sudo dnf remove code

# delete the folders ~/.config/Code and ~/.vscode
```












<br><br>
______________________________________________________
______________________________________________________
<br><br>


# Workflows

<br><br>

## Merge Conflicts

<br><br>

### Deleted files
- Right click on merge conflict and then click stage changes and then click delete file
























<br><br>
______________________________________________________
______________________________________________________
<br><br>



# Extensions
Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.

```bash
ext install  fabiospampinato.vscode-terminals DanielSanMedium.dscodegpt ryu1kn.partial-diff mikestead.dotenv traBpUkciP.vscode-npm-scripts shalldie.background dbaeumer.vscode-eslint abiospampinato.vscode-monokai-night hoovercj.vscode-power-mode be5invis.vscode-custom-css eamodio.gitlens TabNine.tabnine-vscode tonybaloney.vscode-pets ms-azuretools.vscode-docker TheCodemonkey.synthwave-x-fluoromachine-epic-animations stevencl.addDocComments vikas.code-navigation stevencl.addDocComments gencay.vscode-chatgpt ms-vscode.live-server leodevbro.blockman usernamehw.errorlens s-nlf-fh.glassit ChakrounAnas.turbo-console-log
```

<br><br>

// OpenAI
- Get API key here: https://beta.openai.com/account/api-keys
- https://marketplace.visualstudio.com/items?itemName=DanielSanMedium.dscodegpt

<br><br>
- https://marketplace.visualstudio.com/items?itemName=leodevbro.blockman
- https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server
- https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens
- https://marketplace.visualstudio.com/items?itemName=s-nlf-fh.glassit
- https://marketplace.visualstudio.com/items?itemName=ChakrounAnas.turbo-console-log

- https://marketplace.visualstudio.com/items?itemName=ryu1kn.partial-diff
- https://marketplace.visualstudio.com/items?itemName=stevencl.addDocComments
- https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode
- https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.intellicode-api-usage-examples
- https://marketplace.visualstudio.com/items?itemName=oouo-diogo-perdigao.docthis
- https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv
- https://marketplace.visualstudio.com/items?itemName=traBpUkciP.vscode-npm-scripts
- https://marketplace.visualstudio.com/items?itemName=shalldie.background
- https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
```
# Run inside your project
npm i -dev eslint
eslint --init
```

- https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-monokai-night
- https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-power-mode
- https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css
- https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens
- https://marketplace.visualstudio.com/items?itemName=TabNine.tabnine-vscode
- https://marketplace.visualstudio.com/items?itemName=tonybaloney.vscode-pets
- https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker
- https://marketplace.visualstudio.com/items?itemName=vikas.code-navigation
- https://marketplace.visualstudio.com/items?itemName=gencay.vscode-chatgpt
- https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-terminals
```
The extension would NOT work if Visual Studio Code cannot modify itself. The cases include:

Code files being read-only, like on a read-only file system or,
Code is not started with the permissions to modify itself.
You need to claim ownership on Visual Studio Code's installation directory, by running this command:

sudo chown -R $(whoami) <Path to Code>
The placeholder <Path to Visual Studio Code> means the path to VSCode installation. It is typically:

/Applications/Visual Studio Code.app/Contents/MacOS/Electron, on MacOS;
/Applications/Visual Studio Code - Insiders.app/Contents/MacOS/Electron, on MacOS when using Insiders branch;
/usr/share/code, on most Linux;
/usr/lib/code/ or /opt/visual-studio-code on Arch Linux.
Mac and Linux package managers may have customized installation path. Please double check your path is correct.
```
- https://marketplace.visualstudio.com/items?itemName=TheCodemonkey.synthwave-x-fluoromachine-epic-animations
```
  // For Linux it would be in your settings.json
  "vscode_custom_css.imports": [
    "file:////home/CyberT33N/.vscode/extensions/thecodemonkey.synthwave-x-fluoromachine-epic-animations-1.4.13/synthwave-x-fluoromachine.itermcolors",
    "file:////home/CyberT33N/.vscode/extensions/thecodemonkey.synthwave-x-fluoromachine-epic-animations-1.4.13/epic-80s-transitions.css"
    ],
```















<br><br>
<br><br>


# Keybindings
- Open File > Preferences > Keyboard Shortcuts

<br><br>

## Switch Windows
- The workbench.action.switchWindow keybinding to select the window to switch to. It is bound to ctrl+w by default
  - The workbench.action.quickSwitchWindow command. Unlike workbench.action.switchWindow, it automatically switches windows when you release the keys. It is not bound by default but you can configure a keybinding for it.

<br><br>

## Open specific file new window
```shell
On Windows and Linux, press CTRL+K, then release the keys and press O (the letter O, not Zero).

On macOS, press CMD+K, then O (without holding CMD).

This will open the active file tab in a new window/instance.
```

























<br><br>
<br><br>

____________________________________________________
____________________________________________________

<br><br>
<br><br>



# Terminals Manager
1. Shift + P 
  - Terminals: Edit Configuration
```javascript
{
  "autorun": true,
  "autokill": true,
  "terminals": [
    {
      "name": "project 1",
      "description": "test",
      "execute" : true,
      "focus": true,
      "commands": [
        "cd servers/ccs",
        "npm run start-dev"
      ]
    },
    {
      "name": "ui",
      "execute" : true,
      "commands": [
        "cd ui/ccs",
        "sencha app watch"
      ]
    }
  ]
}
```
2. Shift + P
  -  Terminals: Run












<br><br>
<br><br>


# Settings
- Open ~/.config/Code/User/settings.json

<br><br>

## Monokai Dark Thema
```javascript
{
    "workbench.colorTheme": "Monokai Night",
    "workbench.iconTheme": "Monokai Pro (Filter Octagon) Icons",
    "workbench.colorCustomizations": {
        "editor.background": "#1a1a1a",
    },

    "files.autoSave": "afterDelay",

    "editor.tokenColorCustomizations": {
        "variables": "#ffffff",
        "textMateRules": [
            {
                "scope": "storage.type.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "storage.type.function.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "meta.var-single-variable.expr.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                    }
            },
            {
                "scope": "variable.other.readwrite.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                    }
            },
            {
                "scope": "constant.language.boolean.false.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "punctuation.separator.dictionary.key-value.json.comments",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "variable.language.this.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "support.type.property-name.json",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                    }
            },
            {
                "scope": "string.quoted.double.json.comments",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#ffe600"
                    }
            },
            {
                "scope": "string.quoted.single.js",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#ffe600"
                    }
            },
            {
                "scope": "storage.type.function.arrow.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "meta.brace.square.js",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "punctuation.definition.dictionary.begin.json.comments",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "punctuation.definition.dictionary.end.json.comments",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "punctuation.definition.array.begin.json.comments",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "punctuation.definition.array.end.json.comments",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "constant.language.undefined.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "keyword.control.loop.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ff0000"
                    }
            },
            {
                "scope": "constant.language.boolean.true.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                    }
            },
            {
                "scope": "meta.block.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                    }
            },
            {
                "scope": "variable.other.constant.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                    }
            }
        ]
     },
    "editor.fontSize": 16,
    "editor.tabSize": 5,
    "editor.fontFamily": "'Fira Code', 'monospace', monospace",
    "editor.wordWrap": "on",
    "editor.bracketPairColorization.independentColorPoolPerBracketType": false,
    "editor.codeLensFontSize": 17,
    "editor.letterSpacing": 0.5,
    "editor.mouseWheelZoom": true,
    "editor.smoothScrolling": true,
    "editor.cursorBlinking": "smooth",
    "editor.cursorSmoothCaretAnimation": false,
    "editor.cursorStyle": "line-thin",
    "editor.fontLigatures": true,
    "editor.fontWeight": "bold",
    "editor.minimap.scale": 2,
    "editor.minimap.size": "fit",

    "workbench.list.smoothScrolling": true,
    "workbench.preferredDarkColorTheme": "Monokai Dimmed",
    "debug.allowBreakpointsEverywhere": true,
    "debug.console.fontFamily": "'Fira Code', 'monospace', monospace",
    "terminal.integrated.scrollback": 50000,
    "telemetry.telemetryLevel": "off",
    "eslint.alwaysShowStatus": true,
    "eslint.useESLintClass": true,
    "editor.bracketPairColorization.enabled": false
}
```





































<br><br>

## Legends Theme
- https://github.com/CyberT33N/vs-code-legends-theme






















<br><br>
<br><br>



## Syntax Highlighting

#### Custom edits
- editor.tokenColorCustomizations can use a number of values: comments, functions, keywords, numbers, strings, types and variables. If none of those work for you textMateRules is available as well. So you can do something like:
```javascript
"editor.tokenColorCustomizations": {
    "textMateRules": [{
        "scope": "yourScopeHere",
        "settings": {
            "fontStyle": "italic",
            "foreground": "#C69650"
        }
    }]
   }
```
So you just have to figure out what scope you need for "interface".

For that, try CTRL-Shift-P and type scope: choose
- Developer: Inspect Editor Tokens and Scopes  

and for whichever keyword is selected, like interface you will get a listing of its textmate scope. That should be inserted as the scope value above. [In my experience, it is more accurate to open the "Inspect TM Scopes" panel and then click a couple of items and then the one, like interface, that you want - the scope panel will remain open.] You can copy from the scopes panel.

You may need only the main scope listed, but if need to narrow its scope you can include the others listed in a comma-separated list in the scopes: ..., ..., ...





















<br><br>
<br><br>
__________________________________________________________
__________________________________________________________
<br><br>
<br><br>




# Debug
- https://code.visualstudio.com/docs/nodejs/nodejs-debugging#_javascript-debug-terminal

## Automatically start all npm run command in debug mode:
- Ctrl+Shift+P -> Toogle Auto Attach -> Always

## Extensions

### Run npm scripts from package.json with 1-click from your sidebar
- View - Open View -> NPM Scripts
































<br><br>
<br><br>
__________________________________________________________
__________________________________________________________
<br><br>
<br><br>





# Terminal


<br><br>
<br><br>



## Auto open each start
You just need to add a terminals.json file in your workspace (under .vscode) with something like this, and set autorun to true. This would auto-run the extension's Terminals: Run command on startup to auto-load your terminals.
```javascript
{
    "autorun": true,
    "autokill": true,
    "terminals": [
        {
            "name": "GIT",
            "description": "For running git commands",
            "open": true,
            "focus": true,
            "commands": [
                "pwd",
                "git fetch -v"
            ]
        },
        {
            "name": "BUILD",
            "description": "For running build commands",
            "open": true,
            "focus": false,
            "commands": [
                "cd apps",
                "./clean.sh"
            ]
        },
        {
            "name": "SCRIPTS",
            "description": "For running python commands",
            "open": true,
            "focus": false,
            "commands": [
                "source $VENV_DIR/test-py38/bin/activate",
                "python -V"
            ]
        },
    ]
}
```



























<br><br>
<br><br>
__________________________________________________________
__________________________________________________________
<br><br>
<br><br>




# Hotkeys

<br><br>

## Comment out Code
- CTRL + SHIFT + /

