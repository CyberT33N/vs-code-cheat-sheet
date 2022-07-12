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
```javascript
{
    "workbench.colorTheme": "Synthwave x Fluoromachine & epic animations",
    "workbench.iconTheme": "material-icon-theme",

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

    "workbench.colorCustomizations": {
        "editor.background": "#1a1a1a",
    },
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
    "git.mergeEditor": true
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
    color: turquoise;
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

