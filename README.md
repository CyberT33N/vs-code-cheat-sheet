# VS Code Cheat Sheet
VS Code Cheat Sheet with the most needed stuff..



# Extensions
- https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
- https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-monokai-night

<br><br>
<br><br>


# Settings
- Open ~/.config/Code/User/settings.json

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
                    "fontStyle": "",
                    "foreground": "#E6DB74"
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



