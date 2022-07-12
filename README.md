# VS Code Cheat Sheet
VS Code Cheat Sheet with the most needed stuff..

<br><br>

# Extensions
- https://marketplace.visualstudio.com/items?itemName=shalldie.background
- https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
- https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-monokai-night
- https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-power-mode
- https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css
- https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens
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
<br><br>

____________________________________________________
____________________________________________________

<br><br>
<br><br>
















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

## Synthwave x Fluoromachine & epic animations

settings.json
```javascript
{
    "workbench.colorTheme": "Synthwave x Fluoromachine & epic animations",
    "workbench.iconTheme": "material-icon-theme",

    "workbench.colorCustomizations": {
        "editor.background": "#1a1a1a",
        "scrollbarSlider.background": "#ffca28c9",
        "scrollbarSlider.hoverBackground": "#ffca28",
        "scrollbarSlider.activeBackground": "#ffca28c9",
    },
    
    "powermode.enabled": true,
    "powermode.presets": "flames",
    "powermode.combo.counterSize": 1,
    "powermode.shake.enabled": false,

    
    "workbench.editor.enablePreview": false,
    
    "background.enabled": true,
    "background.loop": true,
    "background.useDefault": false,
    "background.useFront": false,
    "background.style": {
          "content": "''",
          "pointer-events": "none",
          "position": "absolute",
          "z-index": "99999",
          "width": "100%",
          "height": "100%",
          "background-size": "cover",
          "background-repeat": "no-repeat",
          "opacity": 0.1
      },
    "background.customImages": [
          "https://preview.redd.it/0bb6dqsiab451.gif?s=b0c65596a54a30708da26669da6e79abf3be1680",
          "https://media2.giphy.com/media/gQvJdypeqrEyhZ9lzn/giphy.gif?cid=790b76118cd8aa4ef3ff335d2f602093346b6391cf3bdbae&rid=giphy.gif"
      ],

    "vscode_custom_css.imports": [
        "file:////home/dennis/.vscode/extensions/thecodemonkey.synthwave-x-fluoromachine-epic-animations-1.4.13/synthwave-x-fluoromachine.itermcolors",
        "file:////home/dennis/.vscode/extensions/thecodemonkey.synthwave-x-fluoromachine-epic-animations-1.4.13/epic-80s-transitions.css"
    ],
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
                "scope": "punctuation.definition.string.begin.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "meta.object-literal.key.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "punctuation.definition.string.end.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
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
                "scope": "punctuation.definition.section.case-statement.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "punctuation.definition.block.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "string.quoted.double.yaml",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fffb00"
                }
            },
            {
                "scope": "string.quoted.double.json",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fffb00"
                }
            },            
            {
                "scope": "entity.name.tag.yaml",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "punctuation.definition.string.begin.json.comment",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "punctuation.separator.key-value.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.operator.ternary.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.operator.expression.typeof.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.control.trycatch.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.control.with.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "entity.name.tag.yaml",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "storage.type.class.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.operator.relational.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "punctuation.separator.dictionary.key-value.json",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },

            {
                "scope": "keyword.control.flow.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "variable.parameter",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ff9900"
                }
            },
            {
                "scope": "entity.name.function.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#9dff00"
                }
            },
            {
                "scope": "support.function",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#9dff00"
                }
            },
            {
                "scope": "entity.name.function.member",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#9dff00"
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
                "scope": "variable.other.property.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "punctuation.definition.parameters.begin.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "punctuation.definition.parameters.end.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "support.variable.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "string.quoted.single.js",
                "settings": {
                    "fontStyle": "italic bold",
                    "foreground": "#fffb00"
                }
            },
            {
                "scope": "string.quoted.single.yaml",
                "settings": {
                    "fontStyle": "italic bold",
                    "foreground": "#fffb00"
                }
            },
            {
                "scope": "string.quoted.double.js",
                "settings": {
                    "fontStyle": "italic bold",
                    "foreground": "#fffb00"
                }
            },
            {
                "scope": "string.template.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fffb00"
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
                "scope": "punctuation.definition.string.template.begin.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "punctuation.definition.string.template.end.js",
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
                "scope": "punctuation.definition.template-expression.begin.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#11f2fa"
                }
            },
            {
                "scope": "punctuation.definition.template-expression.end.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#11f2fa"
                }
            },
            {
                "scope": "keyword.operator.comparison.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.control.conditional.js",
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
                "scope": "constant.numeric.decimal.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ac46ff"
                }
            },
            {
                "scope": "punctuation.separator.array.json.comments",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "punctuation.separator.dictionary.pair.json.comments",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#ffffff"
                }
            },
            {
                "scope": "meta.structure.dictionary.value.json.comments",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#ffe600"
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
                "scope": "punctuation.definition.string",
                "settings": {
                    "fontStyle": "bold",
                    "foreground": "#fff"
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
                    "foreground": "#fff"
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
                "scope": "variable.other.constant.property.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "support.variable.property",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "support.class",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#0066ff"
                }
            },
            {
                "scope": "entity.name.type.class.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#0066ff"
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
                "scope": "keyword.operator.new.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.operator.assignment.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.operator.logical.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "entity.name.type.module.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "meta.brace.round.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fff"
                }
            },
            {
                "scope": "keyword.operator.arithmetic.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "keyword.control.switch.js",
                "settings": {
                    "fontStyle": "",
                    "foreground": "#fa115f"
                }
            },
            {
                "scope": "storage.modifier.async.js",
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
            },
            {
                "scope": "punctuation.accessor.js",
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
    "editor.bracketPairColorization.enabled": false,
    "merge-conflict.autoNavigateNextConflict.enabled": true,
    "git.mergeEditor": true,
    "editor.scrollbar.vertical": "visible"
}
```

epic-80s-transitions.css
```javascript
@import url('https://fonts.googleapis.com/css2?family=Tourney:ital,wght@1,100&display=swap');


/* hover flip specials */


.mtk8, .mtk9, .mtk3, .mtk6, .mtk7, .mtk10 {
    display: inline-block;
    
    transition: .4s transform;
    /* transform: rotateX(0); */
}

/*
.mtk8:hover, .mtk9:hover, .mtk3:hover, .mtk6:hover, .mtk7:hover, .mtk10:hover {
    text-shadow: 2 2 15px;
    transform: scale(1.2);
}*/


/* end of hover flip specials */


/* tooltips */

.monaco-editor .monaco-hover {
    background-color: #262335;
    display: block!important;
    padding: 20px;
    transition: opacity 1s !important;
    opacity: 1;
    animation: tooltippulse 4s infinite linear;
}

.monaco-editor .monaco-hover.hidden {
    opacity: 0;
}

@keyframes tooltippulse {
    0% {  
        box-shadow: 0 0 0 0 rgba(255, 0, 242, 0);   
    }
    50% {
        box-shadow: 0 0 85px 0 rgba(0, 217, 255, 0.5);  
    }
    100% {
        box-shadow: 0 0 0 0 rgba(255, 0, 242, 0);
    }    
}
/*
.monaco-editor .monaco-hover::after {
    content: '';
    position: absolute;
    bottom: -1px;
    left: 0;
    right: 0;
    height: 4px;
    background-size: 200% 200%;
    width: 100%;
    background-image: linear-gradient(to right, #fc28a8, #03edf9, #fc28a8, #03edf9, #fc28a8);

    animation: neonline 2s infinite;
}*/

@keyframes neonline {
    0% {  
       background-position: 0% 50%;
    }
    100% {
        background-position: 100% 50%;
    }    
}



/* end of tooltips */


/* tabs */

/* .monaco-workbench .part.editor>.content .editor-group-container>.title .tabs-container>.tab.active::before {
    
    animation: neonline2 2s infinite;
    background-size: 200% 200%!important;
    width: 100%;
    background-image: linear-gradient(to right, #fc28a8, #03edf9, #fc28a8, #03edf9, #fc28a8)!important;
}

@keyframes neonline2 {
    0% {  
       background-position: 0% 50%;
    }
    100% {
        background-position: 100% 50%;
    }    
} */

/* end of tabs*/


.monaco-editor .selected-text {
    background-color: #ffffff69 !important;
    box-shadow: 0 0 35px 5px #ff008d55;
    color: #fff !important;
 }


.monaco-editor .cursor { 
    box-shadow: 0 0 15px 2px #00c3ff;
    animation: cursor .5s infinite linear;
}


.editor-group-container:after {
    animation: flight 2s infinite linear;
}

.view-line .inline-folded:after {
    color:yellow;
    border-radius: 5px;
    animation: colapse .5s linear;
}



.monaco-editor .line-numbers.active-line-number {
    color: #ffca28;
    text-shadow: 0 0 1px yellow!important;
}




/* canvas.minimap-decorations-layer {
    background-color: transparent !important;
    background-image: linear-gradient(to bottom, #200933 75%, #3d0b43);
    background-size: auto 100vh;
    background-position: top;
    background-repeat: no-repeat;
} */

.monaco-editor .minimap-shadow-visible {
    box-shadow: none!important;
}





@keyframes colapse {
    0% {  
        background-color:yellow;
        box-shadow: 0 0 5px 0 yellow;      
    }
    70% {
        background-color: yellow;
        box-shadow: 0 0 35px 10px yellow;
    }
    100% {
        background-color: transparent;
    }    
}

@keyframes cursor {
    0% {  
        box-shadow: 0 0 5px 0 #00c3ff;      
    }
    100% {
        box-shadow: 0 0 35px 5px #00c3ff;
    }
}

@keyframes flight {
  0% {
    transform: perspective(100px) rotateX(60deg) translateY(0px);
  }
  100% {
    transform: perspective(100px) rotateX(60deg) translateY(20px);
  }
}



.editor-container::after {
    display: flex;
    align-items: center;
    align-content: center;
    justify-content: center;

    /* content: 'do epic shit...'; */
    content: ' ';
    font-weight: bold;
    font-size: 5em;
    font-family: 'Tourney', cursive;

    color: #fc28a822;
    position: absolute;
    bottom: 40px;
    width: 100%;
    overflow-x: hidden;
    height: 120px;
    

    text-shadow: 0 0 30px #fc28a8;

    animation: cnt 10s infinite linear;



}

@keyframes cnt {
    0% {  
        bottom: 150px;
        font-size: 0.1em;
        color: #fc28a822;       
        text-shadow: 0 0 5px #fc28a811;
    }
    100% {
        bottom: -400px;
        font-size: 20em;       
        color: #fc28a855;
        text-shadow: 0 0 30px #fc28a8;
    }
}
```


synthwave-x-fluoromachine.css
```javascript
:root {
  font-smooth: always;
}

.mtk3, .mtk6 {
  color: #61e2ff;
  text-shadow: 0 0 2px #001716, 0 0 5px #03edf933, 0 0 10px #ffff6633;
}

.mtk3.mtki {
  font-style: italic;
  color: #9963ff99;
}

.mtk4, .mtk5, .mtk11, .mtk14 {
  color: #9963ff;
}

.mtk8, .mtk9 {
  /* color: #fd8902; */
  color: #ffcc00;
  text-shadow: 0 0 2px #100c0f, 0 0 3px #ffaa0099, 0 0 5px #ffaa0099, 0 0 10px #ffaa0099;
  font-style: italic;
}

/* .mtk7 {
  color: #8a2dc0;
  text-shadow: 0 0 2px #000, 0 0 10px #8a2dc066, 0 0 5px #8a2dc066, 0 0 25px #8a2dc066;
} */

/* .mtk8 {
  color: #72f1b8;
  text-shadow: 0 0 2px #100c0f, 0 0 10px #257c55, 0 0 35px #212724;
} */

.mtk7, .mtk10 {
  color: #fc199a;
  text-shadow: 0 0 2px #393a33, 0 0 35px #ffffff44, 0 0 10px #fc199a, 0 0 2px #fc199a;
}


.mtk10 {
    font-style: italic;
}

.monaco-editor .margin, .monaco-editor-background, .monaco-editor .inputarea.ime-input {
  background: transparent;
}

.monaco-workbench .part.editor > .content .editor-group-container.empty .editor-group-letterpress {
  background-image: url("data:image/svg+xml,%3C%3Fxml version='1.0' encoding='UTF-8'%3F%3E%3Csvg width='41px' height='40px' viewBox='0 0 41 40' version='1.1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink'%3E%3Cdefs%3E%3ClinearGradient x1='50%25' y1='0%25' x2='50%25' y2='97.6652818%25' id='linearGradient-1'%3E%3Cstop stop-color='%23FC28A8' offset='0%25'%3E%3C/stop%3E%3Cstop stop-color='%2303EDF9' offset='100%25'%3E%3C/stop%3E%3C/linearGradient%3E%3C/defs%3E%3Cg id='Page-1' stroke='none' stroke-width='1' fill='none' fill-rule='evenodd'%3E%3Cg id='letterpress-dark' fill='url(%23linearGradient-1)'%3E%3Cg id='Group'%3E%3Cpath d='M30.2354,39.8836 C29.9195,39.8862 29.6057,39.8287 29.3109,39.7139 C28.9896,39.5885 28.6977,39.3979 28.4539,39.1539 L12.6999,24.7799 L9.23917,27.4037 L5.83434,29.986 C5.70454,30.0845 5.56201,30.1626 5.41164,30.2189 C5.20259,30.2976 4.9783,30.3339 4.7519,30.3239 C4.36361,30.3068 3.99356,30.1543 3.70588,29.8929 L1.50588,27.8929 C1.33452,27.7368 1.19763,27.5466 1.10396,27.3346 C1.01029,27.1225 0.961914,26.8933 0.961914,26.6614 C0.961914,26.4296 1.01029,26.2004 1.10396,25.9883 C1.19763,25.7762 1.33452,25.5861 1.50588,25.4299 L7.45788,19.9999 L4.67072,17.4532 L1.50734,14.5689 C1.33584,14.4129 1.19883,14.2227 1.10507,14.0107 C1.01132,13.7986 0.962891,13.5693 0.962891,13.3374 C0.962891,13.1056 1.01132,12.8763 1.10507,12.6642 C1.19883,12.4521 1.33584,12.262 1.50734,12.1059 L3.70734,10.1059 C3.72926,10.086 3.75165,10.0667 3.7745,10.048 C4.05213,9.82027 4.39666,9.68789 4.7569,9.67196 C5.14519,9.65479 5.52725,9.77401 5.83688,10.0089 L12.6999,15.2179 L28.4519,0.843942 C28.5452,0.751682 28.6455,0.666763 28.7519,0.589942 C29.1153,0.325601 29.5436,0.164633 29.9911,0.124137 C30.0919,0.11502 30.1928,0.112086 30.2933,0.115234 C30.6444,0.123748 30.9918,0.206443 31.3117,0.360027 L39.5477,4.32103 C39.9716,4.52522 40.3292,4.84487 40.5795,5.24325 C40.7787,5.56023 40.9035,5.9168 40.9462,6.28629 C40.9574,6.38148 40.9632,6.47754 40.9633,6.57401 L40.9633,6.67295 C40.9633,6.65781 40.9631,6.64268 40.9627,6.62757 L40.9627,33.3704 C40.9631,33.3552 40.9633,33.3401 40.9633,33.3249 L40.9633,33.4199 C40.9633,33.5146 40.9579,33.609 40.9472,33.7025 C40.9055,34.0754 40.7802,34.4355 40.5793,34.7552 C40.329,35.1534 39.9714,35.4729 39.5477,35.677 L31.3117,39.638 C31.0191,39.7785 30.7037,39.8596 30.3833,39.879 C30.3341,39.882 30.2848,39.8835 30.2354,39.8836 Z M30.9509,10.9369 L19.0028,19.9987 L30.9549,29.0639 L30.9509,10.9369 Z' id='Shape'%3E%3C/path%3E%3C/g%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
  position: relative;
}

/* Add the subtle gradient to the editor background */
.editor .content, .monaco-editor {
  background-color: transparent !important;
  background-image: linear-gradient(to bottom, #200933 75%, #3d0b43);
  background-size: auto 100vh;
  background-position: top;
  background-repeat: no-repeat;
  position: relative;
}

.editor-container {
    position: relative;
    overflow: hidden;
}

.editor-group-container:after{
  content:'';
  height:300px;
  width:100%;
  display:block;
  background-image:linear-gradient(90deg, rgba(252,25,154,.1) 1px, rgba(0,0,0,0) 1px), linear-gradient(0deg, rgba(252,25,154,.1) 1px, rgba(0,0,0,0) 1px);
  background-position:bottom;
  background-repeat:repeat;
  background-size:20px 20px;
  left: -25px;
  position: absolute;
  pointer-events: none;
  bottom: 0;
  transform: perspective(100px) rotateX(60deg);
  z-index: 0;
}
.editor-group-container {
  position: relative;
  overflow: hidden;
}

/* .monaco-editor > .overflow-guard > .monaco-scrollable-element:before { */
.monaco-editor:before, .editor-group-container:before {
    background-image: repeating-linear-gradient(to bottom, transparent 0 ,transparent 2px, #FFF 2px, #FFF 4px);
    background-size: 100% 4px cover;
    transform-origin: 50% 50%;
    content: '';
    opacity: 0.02;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
}

/* .monaco-editor .overflow-guard .margin {
    background: #210A33;
} */

canvas {
    z-index: 2; 
}

.minimap-slider {
    z-index: 3;
    background: #fc199a33 !important;
}

.minimap.slider-mouseover {
    z-index: 1;
}

/* Sweet sunset dots */
.monaco-workbench .activitybar>.content .monaco-action-bar .badge .badge-content {
  background: linear-gradient(to bottom, #fff951 25%, #fc28a8);
}

.monaco-workbench .part.editor>.content .editor-group-container>.title .tabs-container>.tab.sizing-fit::after {
  content: '';
  position: absolute;
  bottom: -1px;
  left: 0;
  right: 0;
  height: 0px;
  transition: opacity 1s;
  opacity: 0;
}

/* Active sidebar item */
.monaco-workbench .activitybar>.content .monaco-action-bar .action-item.checked {
  box-shadow: inset 0 -5px 25px #fc28a825;
  position: relative;
}

.monaco-workbench .activitybar>.content .monaco-action-bar .action-item.checked::after {
  content: '';
  position: absolute;
  bottom: 0px;
  top: 0px;
  left: 0px;
  width: 4px;
  background: linear-gradient(to bottom, #fc28a8, #03edf9) !important;
  opacity: 1;
}

.monaco-workbench .activitybar>.content .monaco-action-bar .action-item::after {
  content: '';
  position: absolute;
  bottom: 0px;
  top: 0px;
  left: 0px;
  width: 0px;
  transition: opacity 1s;
  opacity: 0;
}

/* Active tab neon */
.monaco-workbench .part.editor>.content .editor-group-container>.title .tabs-container>.tab.active {
  position: relative;
  --tab-border-bottom-color: transparent !important;
}

/* Active tab stripe */
.monaco-workbench .part.editor>.content .editor-group-container>.title .tabs-container>.tab.active::before {
  content: '';
  position: absolute;
  bottom: -1px;
  left: 0;
  right: 0;
  height: 4px;  
  background: linear-gradient(to right, #fc28a8, #03edf9) !important;
}

/* update lightbulb to be neon */
.lightbulb-glyph {
  background:  url("data:image/svg+xml,%3Csvg id='Layer_1' data-name='Layer 1' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3E%3Crect fill='%23ffffff' x='5.68' y='6.93' width='2.1' height='6.1' rx='0.96' transform='translate(-1.94 1.63) rotate(-12.09)'/%3E%3Cpath fill='%2303edf9' d='M7.08,13.5a1.46,1.46,0,0,1-1.43-1.16L4.77,8.26A1.47,1.47,0,0,1,5.9,6.53l.17,0A1.46,1.46,0,0,1,7.81,7.61l.87,4.09a1.46,1.46,0,0,1-1.12,1.73l-.18,0Zm-.7-6h-.1l-.17,0a.45.45,0,0,0-.29.21.45.45,0,0,0-.07.34l.88,4.09a.46.46,0,0,0,.54.35l.18,0a.46.46,0,0,0,.29-.2.48.48,0,0,0,.07-.35L6.83,7.82A.46.46,0,0,0,6.38,7.46Z'/%3E%3Crect fill='%23ffffff' x='8.22' y='6.93' width='2.1' height='6.1' rx='0.96' transform='translate(16.25 21.68) rotate(-167.91)'/%3E%3Cpath fill='%2303edf9' d='M8.93,13.5a1.63,1.63,0,0,1-.31,0l-.18,0A1.46,1.46,0,0,1,7.32,11.7l.87-4.09A1.47,1.47,0,0,1,9.93,6.49l.18,0a1.45,1.45,0,0,1,.92.63,1.47,1.47,0,0,1,.2,1.1l-.88,4.08a1.45,1.45,0,0,1-.63.93A1.48,1.48,0,0,1,8.93,13.5Zm.69-6a.45.45,0,0,0-.25.07.5.5,0,0,0-.2.29L8.3,11.9a.43.43,0,0,0,.06.35.46.46,0,0,0,.29.2l.18,0a.47.47,0,0,0,.55-.35l.87-4.09a.45.45,0,0,0-.06-.34A.47.47,0,0,0,9.9,7.5l-.18,0Z'/%3E%3Cpath fill='%23ffffff' d='M11.77,9l-3.53.67a1,1,0,0,1-1.15-.88h0A1.09,1.09,0,0,1,7.9,7.48l3.53-.67a1,1,0,0,1,1.15.89h0A1.08,1.08,0,0,1,11.77,9Z'/%3E%3Cpath fill='%2303edf9' d='M8.07,10.18A1.54,1.54,0,0,1,6.6,8.83a1.74,1.74,0,0,1,.25-1.22,1.46,1.46,0,0,1,1-.66l3.52-.67A1.51,1.51,0,0,1,13.07,7.6a1.61,1.61,0,0,1-1.22,1.88l-3.52.67A1.15,1.15,0,0,1,8.07,10.18ZM11.6,7.34h-.09L8,8a.53.53,0,0,0-.4.62.5.5,0,0,0,.57.44l3.52-.67a.54.54,0,0,0,.41-.62A.53.53,0,0,0,11.6,7.34Z'/%3E%3Cpath fill='%23ffffff' d='M11.74,6.74,4.67,8.08A1,1,0,0,1,3.52,7.2h0A1.08,1.08,0,0,1,4.33,6l7.06-1.34a1,1,0,0,1,1.16.88h0A1.08,1.08,0,0,1,11.74,6.74Z'/%3E%3Cpath fill='%2303edf9' d='M4.5,8.64a1.44,1.44,0,0,1-.86-.29A1.64,1.64,0,0,1,3,7.29a1.72,1.72,0,0,1,.25-1.21,1.48,1.48,0,0,1,1-.67l7.07-1.34a1.39,1.39,0,0,1,1.11.27A1.65,1.65,0,0,1,13,5.4a1.72,1.72,0,0,1-.25,1.21,1.48,1.48,0,0,1-1,.67L4.76,8.62Zm7.07-3.5h-.09L4.42,6.49a.45.45,0,0,0-.32.22.56.56,0,0,0-.09.4.61.61,0,0,0,.21.35.47.47,0,0,0,.36.09L11.65,6.2A.47.47,0,0,0,12,6a.51.51,0,0,0,.08-.4.55.55,0,0,0-.2-.35A.47.47,0,0,0,11.57,5.14Z'/%3E%3Cpath fill='%23ffffff' d='M11.7,4.52,4.64,5.86A1,1,0,0,1,3.49,5h0A1.09,1.09,0,0,1,4.3,3.72l7.06-1.34a1,1,0,0,1,1.15.88h0A1.09,1.09,0,0,1,11.7,4.52Z'/%3E%3Cpath fill='%2303edf9' d='M4.46,6.42a1.36,1.36,0,0,1-.85-.3,1.58,1.58,0,0,1-.61-1A1.61,1.61,0,0,1,4.21,3.19l7.07-1.34a1.35,1.35,0,0,1,1.11.27,1.58,1.58,0,0,1,.61,1,1.74,1.74,0,0,1-.25,1.22,1.44,1.44,0,0,1-1,.66L4.72,6.39A1.09,1.09,0,0,1,4.46,6.42Zm7.07-3.51h-.08L4.38,4.26a.53.53,0,0,0-.4.62.5.5,0,0,0,.57.44L11.62,4a.47.47,0,0,0,.32-.22.62.62,0,0,0,.08-.4.56.56,0,0,0-.2-.35A.53.53,0,0,0,11.53,2.91Z'/%3E%3Cpath fill='%23ffffff' d='M8.34,2.89,4.57,3.6a1,1,0,0,1-1.15-.88h0a1.08,1.08,0,0,1,.81-1.25L8,.75a1,1,0,0,1,1.15.89h0A1.08,1.08,0,0,1,8.34,2.89Z'/%3E%3Cpath fill='%2303edf9' d='M4.4,4.16a1.44,1.44,0,0,1-.86-.29,1.69,1.69,0,0,1-.61-1.05A1.74,1.74,0,0,1,3.18,1.6a1.51,1.51,0,0,1,1-.67L7.91.22A1.38,1.38,0,0,1,9,.49a1.58,1.58,0,0,1,.61,1.05,1.74,1.74,0,0,1-.25,1.22,1.47,1.47,0,0,1-1,.66l-3.77.72A1.18,1.18,0,0,1,4.4,4.16ZM8.17,1.28H8.09L4.32,2A.45.45,0,0,0,4,2.23a.51.51,0,0,0-.08.4.55.55,0,0,0,.2.35.49.49,0,0,0,.37.09l3.77-.72a.47.47,0,0,0,.32-.22.62.62,0,0,0,.08-.4.56.56,0,0,0-.2-.35A.53.53,0,0,0,8.17,1.28Z'/%3E%3Cpolygon fill='%231e1e1e' points='5.5 11.1 5.5 11.1 5.5 14.4 7.1 16 9.1 16 10.6 14.4 10.6 11.1 5.5 11.1'/%3E%3Cpath fill='%23c5c5c5' d='M6.5,12h3v1h-3Zm1,3H8.6l.9-1h-3Z'/%3E%3C/svg%3E") 50% no-repeat !important;
  filter: drop-shadow(0 0 5px #03edf9);
}

.monaco-editor .cursor { 
    background: linear-gradient(to bottom, #8a2dc0,  #fc28a8);
    box-shadow: 0 0 5px #fc199a;
    border-color: #8a2dc0; 
    color: #241b2f; 
}

.monaco-inputbox>.wrapper>textarea.input::selection {
  background-color:rgba(255,255,255,0.3);
}

.monaco-editor .line-numbers {
  color: #8a2dc066;
  text-shadow: 0 0 2px #393a33, 0 0 35px #ffffff44, 0 0 10px #8a2dc066, 0 0 2px #8a2dc066;
}

.monaco-list .monaco-list-rows {
  background: rgba(36,27,47) !important;
}

.monaco-list-row.focused, .monaco-list-row.selected {
  background-color: #8a2dc033 !important;
}

.explorer-folders-view span[title~="emphasized"], .monaco-icon-label[title~="emphasized"]::after {
  color: #fc199a;
}

.explorer-folders-view span[title~="problems"], .monaco-icon-label[title~="problems"]::after {
  color: #ffcc00;
}

.vs-dark .monaco-scrollable-element>.scrollbar>.slider {
  background: rgb(153, 99, 255);
  opacity: 0.5;
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









<br><br>
<br><br>


# Debug

## Run npm scripts from package.json with 1-click from your sidebar
- View - Open View -> NPM Scripts

