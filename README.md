# VS Code Cheat Sheet
VS Code Cheat Sheet with the most needed stuff..



## Build
- https://github.com/CyberT33N/vs-code-build-cheat-sheet




<br><br>
<br><br>






# Install
- https://code.visualstudio.com/Download
  - You should not install it via snap because then it is read only and the code from below at extensions will not work
```shell
sudo apt install code
```



<br><br>
<br><br>


# Uninstall
- https://code.visualstudio.com/docs/setup/uninstall

## Windows

f you installed VS Code via the Windows Installer, either the User or System version, use the installer to remove VS Code.

Start menu
Search for Add or Remove Programs and find Visual Studio Code in the Apps > Apps & features list.
Select Uninstall from the actions dropdown on the right side (three vertical dots).
Follow the prompts to uninstall VS Code.

Delete %APPDATA%\Code and %USERPROFILE%\.vscode.

## Ubuntu
```shell
sudo apt purge code
sudo apt autoremove
rm -rf ~/.vscode ~/.config/Code
```

<br><br>

## Fedora
```shell
sudo dnf remove code
sudo apt autoremove
rm -rf ~/.vscode ~/.config/Code
```









<br><br>
<br><br>

<br><br>
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


# Workflows

<br><br>

## Merge Conflicts

<br><br>

### Good 2 Know
Imagine you would do:
```shell
git checkout branchA
git merge --squash branchB
```
- Then **branchA is current** and **branchB is incoming**

<br><br>
<br><br>

### Merge Editor
- **Always double check the bottom final result Window where your results getting combined. For whatever reason when you accept e.g. any code block from the incoming window and clicking on `accept incoming` then you have to choose to click `remove current` from the final result window. Otherwhise you will have the code of incoming and current together in your final result
  - In general it is very anoying to through this process as described above. Even when you click on `accept all from current` then you still have to decide in the final window to `remove incoming`. Here are some alternatives:
    - **Method 1** E.g. click `accept all from current` and then just completly copy your code e.g. from the current window and then paste it to the final Window and then Merge Button.

<br><br>

### Deleted files
- Right click on the deleted file and and then click stage changes (Or click the + Button this will stage aswell) and then click yes
  - If needed check if the file was really deleted but should be doe



































<br><br>
______________________________________________________
______________________________________________________
<br><br>





# jsconfig.json
- https://code.visualstudio.com/docs/languages/jsconfig





































<br><br>
______________________________________________________
______________________________________________________
<br><br>





# settings.json
- `sudo gedit ~/.config/Code/User/settings.json`
- Make sure to install font fira code




# Design t33n
- Make sure to install extension listed above. Thise settings.json is pre designed




<details><summary>Click to expand..</summary>


```javascript
{
     "workbench.iconTheme": "symbols",
     "editor.codeActionsOnSave": {
          "source.fixAll.eslint": "explicit"
     },
     "workbench.colorCustomizations": {
          "editorInlayHint.background": "#00001CCC",
          "editorInlayHint.foreground": "#99FFBBCC",
          "editorInlayHint.parameterBackground": "#00000000",
          "editorInlayHint.parameterForeground": "#f8f4f44f",
          "editorInlayHint.typeBackground": "#08000088",
          "editorInlayHint.typeForeground": "#DDEEFF88",
          "editorHoverWidget.border": "#ffca28",
          "editorHoverWidget.background": "#080808",
          "editorHoverWidget.foreground": "#ffffff",

          "editor.background": "#0c0c0c",
          "editor.selectionBackground": "#b8b8b8",
          "editor.selectionHighlightBackground": "#ffffff54",
          "editor.findMatchBackground": "#135564",
          "editor.findMatchHighlightBackground": "#13556496",
          "editor.lineHighlightBackground": "#ffffff29",

          "editorLineNumber.foreground": "#ffffff40",
          "scrollbarSlider.background": "#ffca28c9",
          "scrollbarSlider.hoverBackground": "#ffca28",
          "scrollbarSlider.activeBackground": "#ffca28c9",
          "terminal.background": "#131212",
          "terminal.foreground": "#dddad6",
          "terminal.selectionBackground": "#fff",
          "terminal.selectionForeground": "#fff",
          "terminalCursor.background": "#D0D0D0",
          "terminalCursor.foreground": "#fbe201",
          "terminal.ansiBlack": "#1D2021",
          "terminal.ansiBrightBlack": "#665C54",
          "terminal.ansiBrightBlue": "#0D6678",
          "terminal.ansiBrightCyan": "#8BA59B",
          "terminal.ansiBrightGreen": "#237e02",
          "terminal.ansiBrightMagenta": "#8F4673",
          "terminal.ansiBrightRed": "#f5f5f5",
          "terminal.ansiBrightWhite": "#FDF4C1",
          "terminal.ansiBrightYellow": "#FAC03B",
          "terminal.ansiBlue": "#fbe201",
          "terminal.ansiCyan": "#8BA59B",
          "terminal.ansiGreen": "#52f014",
          "terminal.ansiMagenta": "#8F4673",
          "terminal.ansiRed": "#FB543F",
          "terminal.ansiWhite": "#A89984",
          "terminal.ansiYellow": "#f5f5f5"
     },
     "workbench.editorAssociations": {
          "*.mdc": "default"
     },
     "workbench.editor.enablePreview": false,


     "background.enabled": true,


     "background.panel":
     {
          "useFront": true,
          "style": {
               // "content": "''",
               // "pointer-events": "none",
               // "position": "absolute",
               // "z-index": "99999",
               // "width": "100%",
               // "height": "100%",
               // "background-size": "cover",
               // "background-repeat": "no-repeat",
               // "opacity": 0.1

               // "background-position": "100% 100%",
               // "background-size": "auto",
          },
          "styles": [
               {},
               {},
               {}
          ],

          "opacity": 0.1,
          // "size": "cover",
          // "position": "center",

          "images": [
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Render%20Digital%20Art%20GIF%20by%20time%20(1).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Loop%20Space%20GIF%20by%20time%20(7).gif",
             ],
          "interval": 300,
          "random": true
     },



     "background.sidebar":
     {
         
     },


     "background.fullscreen": {
          "useFront": true,
          "style": {
               // "content": "''",
               // "pointer-events": "none",
               // "position": "absolute",
               // "z-index": "99999",
               // "width": "100%",
               // "height": "100%",
               // "background-size": "cover",
               // "background-repeat": "no-repeat",
               // "opacity": 0.1

               // "background-position": "100% 100%",
               // "background-size": "auto",
          },
          "styles": [
               {},
               {},
               {}
          ],

          "opacity": 0.1,
          // "size": "cover",
          // "position": "center",

          "images": [
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/animation%20art%20GIF%20by%20xponentialdesign.gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Art%20Glowing%20GIF%20by%20time%20(3).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Art%20Glowing%20GIF%20by%20time%20(5).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Art%20Render%20GIF%20by%20time%20(1).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Art%20Render%20GIF%20by%20time.gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/download%20(1).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/download%20(4).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/download%20(6).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Loop%20Space%20GIF%20by%20time%20(1).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Loop%20Space%20GIF%20by%20time%20(3).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Loop%20Space%20GIF%20by%20time%20(6).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Loop%20Space%20GIF%20by%20time%20(8).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Render%20Digital%20Art%20GIF%20by%20time%20(1).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Render%20Digital%20Art%20GIF%20by%20time%20(3).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Render%20Digital%20Art%20GIF%20by%20time%20(5).gif",
               "file:///C:/Users/denni/OneDrive/Dokumente/backgrounds/Render%20Digital%20Art%20GIF%20by%20time.gif"
             ],
          "interval": 300,
          "random": true
     },


     "files.autoSave": "afterDelay",
     "editor.tokenColorCustomizations": {
          "textMateRules": [
               {
                    "scope": "constant.language.boolean.true.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "punctuation.definition.block.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff94"
                    }
               },
               {
                    "scope": "meta.brace.square.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff94"
                    }
               },
               {
                    "scope": "punctuation.definition.typeparameters.begin.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff70"
                    }
               },
               {
                    "scope": "punctuation.definition.typeparameters.end.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff70"
                    }
               },
               {
                    "scope": "punctuation.accessor.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#767676"
                    }
               },


               
//lena 	 	 		  	
               {
                    "scope": "keyword.operator.expression.typeof.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },

               {
                    "scope": "constant",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },

               
               
               
               {
                    "scope": "constant.language.json.comments",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },


               {
                    "scope": "keyword.control.flow.ts",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },

               {
                    "scope": "keyword.control.trycatch.ts",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },


               




               {
                    "scope": "keyword.operator.arithmetic.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },


               {
                    "scope": "punctuation.definition.template-expression.begin.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff"
                    }
               },
               {
                    "scope": "punctuation.definition.template-expression.end.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff"
                    }
               },


               {
                    "scope": "constant.language.null.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },

               {
                    "scope": "storage.type.interface.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f8b"
                    }
               },

               {
                    "scope": "storage.type.interface.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f8b"
                    }
               },



               {
                    "scope": "keyword.control.type.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f8b"
                    }
               },

  
               {
                    "scope": "keyword.control.export.ts",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },
               
               {
                    "scope": "keyword.control.as.ts",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },
               
               {
                    "scope": "keyword.control.from.ts",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },

               {
                    "scope": "keyword.control.import.ts",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#fa115f"
                    }
               },

               



               {
                    "scope": "constant.language.import-export-all.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },

              

               {
                    "scope": "support.class",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#00e5ffb8"
                    }
               },


               
               {
                    "scope": "support.type.primitive.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "support.type.primitive.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },


               {
                    "scope": "entity.name.type.interface",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },




               {
                    "scope": "support.type",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },

               {
                    "scope": "punctuation.definition.string.begin.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#c0c0c0"
                    }
               },
               {
                    "scope": "punctuation.definition.string.end.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#c0c0c0"
                    }
               },
               {
                    "scope": "punctuation.definition.string.template.begin.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#c0c0c0"
                    }
               },
               {
                    "scope": "punctuation.definition.string.template.end.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#c0c0c0"
                    }
               },


               {
                    "scope": "punctuation.definition.string.begin.json.comments",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#c0c0c0"
                    }
               },
               {
                    "scope": "punctuation.definition.string.end.json.comments",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#c0c0c0"
                    }
               },



               


               {
                    "scope": "keyword.operator.comparison.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "keyword.operator.assignment.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff"
                    }
               },
               {
                    "scope": "string.template.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#FED482"
                    }
               },


               {
                    "scope": "string.quoted.single.ts",
                    "settings": {
                         "fontStyle": "italic underline",
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "string.quoted.double.ts",
                    "settings": {
                         "fontStyle": "italic underline",
                         "foreground": "#FED482"
                    }
               },
               



               {
                    "scope": " keyword.operator.logical.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "variable.language.this.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": " storage.modifier.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f53"
                    }
               },
               {
                    "scope": "cast.expr.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff77"
                    }
               },
               {
                    "scope": "entity.name.type.module.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "storage.type.class.jsdoc",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#636363"
                    }
               },
               {
                    "scope": "comment.block.documentation.js",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#636363"
                    }
               },
               {
                    "scope": "variable.other.jsdoc",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff92"
                    }
               },
               {
                    "scope": "entity.name.type.instance.jsdoc",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "support.type.builtin.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "support.type.builtin.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "storage.type.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.function.arrow.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.function.arrow.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.function.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.function.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.class.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.class.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
           
               {
                    "scope": "storage.type.type.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "storage.type.type.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "entity.name.type.class.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#0066ff"
                    }
               },
               {
                    "scope": "entity.name.type.class.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#0066ff"
                    }
               },
               {
                    "scope": "entity.name.type.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "entity.name.type.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fffb0077"
                    }
               },
               {
                    "scope": "keyword.operator.optional.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ff005583"
                    }
               },
               {
                    "scope": "keyword.operator.optional.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ff005583"
                    }
               },


               {
                    "scope": "entity.name.function.ts",
                    "settings": {
                         "fontStyle": "italic bold",
                         "foreground": "#9dff00"
                    }
               },
               {
                    "scope": "entity.name.function.tsx",
                    "settings": {
                         "fontStyle": "italic bold",
                         "foreground": "#9dff00"
                    }
               },



               
               


               {
                    "scope": "variable.other.readwrite.alias.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffffea"
                    }
               },

          

               {
                    "scope": "meta.object-literal.key.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fff"
                    }
               },
               {
                    "scope": "meta.object-literal.key.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fff"
                    }
               },
       
               {
                    "scope": "meta.type.annotation.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f49"
                    }
               },
               {
                    "scope": "meta.type.annotation.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f49"
                    }
               },
               {
                    "scope": "keyword.operator.type.annotation.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f49"
                    }
               },
               {
                    "scope": "keyword.operator.type.annotation.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f49"
                    }
               },
               {
                    "scope": "constant.language.undefined.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#FA115F"
                    }
               },
               {
                    "scope": "constant.language.undefined.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#FA115F"
                    }
               },
               {
                    "scope": "variable.object.property.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff7e"
                    }
               },
               {
                    "scope": "variable.object.property.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff7e"
                    }
               },


               {
                    "scope": "keyword.operator.type.annotation.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ffffff7e"
                    }
               },

              



               {
                    "scope": "variable.parameter.ts",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ff9900"
                    }
               },
               {
                    "scope": "variable.parameter.tsx",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ff9900"
                    }
               },
               {
                    "scope": "variable.parameter",
                    "settings": {
                         "fontStyle": "italic bold",
                         "foreground": "#ff9900"
                    }
               },


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
                    "scope": "punctuation.definition.string.begin",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fff"
                    }
               },
               {
                    "scope": "punctuation.definition.string.end",
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
                    "scope": "keyword.control.import.js",
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
                    "scope": "entity.name.function.js",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#9dff00"
                    }
               },
               {
                    "scope": "entity.name.function.shell",
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
                    "scope": "constant.numeric",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#ac46ff"
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
                    "scope": "meta.scope.subshell.shell",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fff"
                    }
               },
               {
                    "scope": "keyword.operator.list.shell",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "keyword.operator.logical.shell",
                    "settings": {
                         "fontStyle": "",
                         "foreground": "#fa115f"
                    }
               },
               {
                    "scope": "keyword.control.shell",
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
                         "foreground": "#ffffff"
                    }
               },
               {
                    "scope": "punctuation.definition.dictionary.end.json.comments",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#ffffff"
                    }
               },




               {
                    "scope": "punctuation.definition.array.begin.json.comments",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#ffffff"
                    }
               },
               {
                    "scope": "punctuation.definition.array.end.json.comments",
                    "settings": {
                         "fontStyle": "bold",
                         "foreground": "#ffffff"
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
               },
               {
                    "scope": "html-template.ng.attribute.doctype",
                    "settings": {
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "html-template.ng.exclamation.doctype",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.entities.ampersand",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.entities.semicolon",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.generic",
                    "settings": {
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.events",
                    "settings": {
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "html-template.ng.aria-attribute.prefix",
                    "settings": {
                         "foreground": "#B97AE2"
                    }
               },
               {
                    "scope": "html-template.ng.aria-attribute.suffix",
                    "settings": {
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "html-template.ng.data-attribute.suffix",
                    "settings": {
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "html-template.ng.interpolation.begin",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.interpolation.end",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.logical",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.compound",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.bitwise",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.comparison",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.relational",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.arithmetic",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.expression.operator.navigator",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.animationtrigger.prefix",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "punctuation.definition.ng-binding-name.begin.html",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "punctuation.definition.ng-binding-name.end.html",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.input-binding.second-level",
                    "settings": {
                         "foreground": "#5BD1B9"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.prefix.let",
                    "settings": {
                         "foreground": "#B97AE2"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.prefix.ref",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.suffix.name",
                    "settings": {
                         "foreground": "#FED482"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.prefix.sugar",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.template.prefix",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.control-flow.prefix",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.svg.path.commands",
                    "settings": {
                         "foreground": "#5BD1B9"
                    }
               },
               {
                    "scope": "html-template.ng.tag.colon",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.tag.suffix",
                    "settings": {
                         "foreground": "#5BD1B9"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.colon",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               },
               {
                    "scope": "html-template.ng.attributes.suffix",
                    "settings": {
                         "foreground": "#5BD1B9"
                    }
               },
               {
                    "scope": "html-template.ng.exclamation.dtd",
                    "settings": {
                         "foreground": "#DCE3EA"
                    }
               },
               {
                    "scope": "html-template.ng.occurrence.dtd",
                    "settings": {
                         "foreground": "#7EAEF5"
                    }
               }
          ]
     },
     "editor.tabSize": 5,
     "editor.inlayHints.fontSize": 14,
     "editor.fontSize": 16,

     "editor.inlayHints.fontFamily": "'GeistMono NF'",
     "debug.console.fontFamily": "'GeistMono NF'",
     "terminal.integrated.fontFamily": "'GeistMono NF'",
     "editor.fontFamily": "'GeistMono NF'",
     "editor.fontLigatures": true,
     "editor.fontWeight": "500",

     "editor.wordWrap": "on",
     "editor.bracketPairColorization.independentColorPoolPerBracketType": false,
     "editor.codeLensFontSize": 17,
     "editor.letterSpacing": 0.5,
     "editor.mouseWheelZoom": true,
     "editor.smoothScrolling": true,
     "editor.cursorBlinking": "smooth",
     "editor.cursorSmoothCaretAnimation": "off",
     "editor.cursorStyle": "line-thin",
     "editor.minimap.scale": 2,
     "editor.minimap.size": "fit",
     "workbench.list.smoothScrolling": true,
     "workbench.preferredDarkColorTheme": "Monokai Dimmed",
     "debug.allowBreakpointsEverywhere": true,
     "terminal.integrated.scrollback": 500000,
     "telemetry.telemetryLevel": "off",
     "eslint.useESLintClass": true,
     "editor.bracketPairColorization.enabled": false,
     "merge-conflict.autoNavigateNextConflict.enabled": true,
     "git.mergeEditor": true,
     "editor.scrollbar.vertical": "visible",
     "vscode-pets.position": "explorer",
     "vscode-pets.petColor": "yellow",
     "vscode-pets.petSize": "medium",
     "vscode-pets.petType": "snake",
     "explorer.confirmDelete": false,
     "js/ts.implicitProjectConfig.experimentalDecorators": true,
     "search.useReplacePreview": false,
     "typescript.suggest.autoImports": false,
     "javascript.suggest.autoImports": false,
     "editor.stickyScroll.enabled": true,
     "glassit.alpha": 220,
     "symbols.hidesExplorerArrows": false,
     "eslint.format.enable": true,
     "eslint.rules.customizations": [],
     "debug.disassemblyView.showSourceCode": false,
     "workbench.productIconTheme": "fluent-icons",
     "vscode_custom_css.imports": [
          "file:///home/t33n/.vscode/extensions/brandonkirbyson.vscode-animations-2.0.3/dist/updateHandler.js"
     ],
     "npm.packageManager": "npm",
     "terminal.integrated.defaultProfile.linux": "zsh",
     "terminal.integrated.profiles.linux": {
          "bash": {
               "path": "bash",
               "icon": "terminal-bash",
               "args": [
                    "--login"
               ]
          },
          "zsh": {
               "path": "zsh"
          },
          "fish": {
               "path": "fish"
          },
          "tmux": {
               "path": "tmux",
               "icon": "terminal-tmux"
          },
          "pwsh": {
               "path": "pwsh",
               "icon": "terminal-powershell"
          },
          "zsh (2)": {
               "path": "/usr/bin/zsh"
          }
     },
     "[typescript]": {
          "editor.defaultFormatter": "vscode.typescript-language-features"
     },
     "specstory.helpUsImprove": false,
     "cursor.composer.shouldAllowCustomModes": true,
     "cursor.composer.shouldChimeAfterChatFinishes": true,
     "roo-cline.allowedCommands": [
          "npm test",
          "npm install",
          "tsc",
          "git log",
          "git diff",
          "git show"
     ],
     "terminal.integrated.defaultProfile.windows": "Windows PowerShell",
     "terminal.integrated.profiles.windows": {
          "PowerShell": {
               "source": "PowerShell",
               "icon": "terminal-powershell",
               "path": "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
          },
          "Command Prompt": {
               "path": [
                    "${env:windir}\\Sysnative\\cmd.exe",
                    "${env:windir}\\System32\\cmd.exe"
               ],
               "args": [],
               "icon": "terminal-cmd"
          },
          "Git Bash": {
               "source": "Git Bash"
          },
          "Windows PowerShell": {
               "path": "C:\\windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
          }
     },


     "cursor.general.enableShadowWorkspace": true,
     "vscode-angular-html.angularAnimationTriggerPrefix": "#7EAEF5",
     "vscode-angular-html.angularBindingAttributeDelimiter": "#7EAEF5",
     "vscode-angular-html.angularExpression": "#7EAEF5",
     "vscode-angular-html.angularExpressionOperatorsAndNavigatorsColor": "#DCE3EA",
     "vscode-angular-html.angularOneWayBindingSecondLevelDepth": "#5BD1B9",
     "vscode-angular-html.angularPrefixedAttributesLetPrefix": "#B97AE2",
     "vscode-angular-html.angularPrefixedAttributesRefPrefix": "#7EAEF5",
     "vscode-angular-html.angularPrefixedAttributesVariableName": "#FED482",
     "vscode-angular-html.angularSyntaxSugarAttributesPrefix": "#7EAEF5",
     "vscode-angular-html.angularTemplateVariablePrefix": "#7EAEF5",
     "vscode-angular-html.colorCustomizations": true,
     "vscode-angular-html.dtdDoctypeExclamation": "#DCE3EA",
     "vscode-angular-html.dtdDoctypeQuantifier": "#7EAEF5",
     "vscode-angular-html.htmlDoctypeAttributes": "#FED482",
     "vscode-angular-html.htmlDoctypeExclamation": "#DCE3EA",
     "vscode-angular-html.htmlEntitiesAmpersand": "#DCE3EA",
     "vscode-angular-html.htmlEntitiesSemicolon": "#DCE3EA",
     "vscode-angular-html.htmlEventsAttributes": "#FED482",
     "vscode-angular-html.htmlGenericAttributesFollowedByParameter": "#FED482",
     "vscode-angular-html.ariaAttributePrefix": "#B97AE2",
     "vscode-angular-html.ariaAttributeSuffix": "#FED482",
     "vscode-angular-html.dataAttributeSuffix": "#FED482",
     "vscode-angular-html.svgDAttributePathCommands": "#5BD1B9",
     "vscode-angular-html.xmlAttributeNamespaceDivider": "#7EAEF5",
     "vscode-angular-html.xmlAttributeNamespaceSuffix": "#5BD1B9",
     "vscode-angular-html.xmlTagNamespaceDivider": "#7EAEF5",
     "vscode-angular-html.xmlTagNamespaceSuffix": "#5BD1B9",
     "vscode-angular-html.controlFlowPrefix": "#7EAEF5",
     "update.releaseTrack": "prerelease",
     "workbench.colorTheme": "Lumen",
     "cursor.diffs.useCharacterLevelDiffs": true
}
```

</details>




































<br><br>
______________________________________________________
______________________________________________________
<br><br>



# Extensions
Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.

<br><br>
<br><br>


## Best choice
- https://marketplace.visualstudio.com/items?itemName=ms-playwright.playwright
  
- https://marketplace.visualstudio.com/items/?itemName=bradlc.vscode-tailwindcss

- https://marketplace.visualstudio.com/items?itemName=Nuxt.mdc
  
- https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-speech

- https://marketplace.visualstudio.com/items?itemName=CodeViz.codeviz

- https://marketplace.visualstudio.com/items?itemName=csstools.postcss

- https://marketplace.visualstudio.com/items?itemName=vitest.explorer
  
- https://marketplace.visualstudio.com/items?itemName=ms-kubernetes-tools.vscode-kubernetes-tools
- https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens
- https://marketplace.visualstudio.com/items?itemName=s-nlf-fh.glassit
 
- https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode
```shell
# https://docs.pieces.app/installation-getting-started/linux
sudo snap install pieces-os
sudo snap connect pieces-os:process-control :process-control
sudo snap install pieces-for-developers
pieces-os
pieces-for-developers
```

- https://marketplace.visualstudio.com/items?itemName=miguelsolorio.fluent-icons
- https://marketplace.visualstudio.com/items?itemName=miguelsolorio.symbols

- https://marketplace.visualstudio.com/items?itemName=BrandonKirbyson.vscode-animations

- https://marketplace.visualstudio.com/items?itemName=ryu1kn.partial-diff

- https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv

- https://marketplace.visualstudio.com/items?itemName=shalldie.background

- https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint


```
# Run inside your project
npm i -dev eslint
eslint --init
```

- https://marketplace.visualstudio.com/items?itemName=aefly.lumen
- https://marketplace.visualstudio.com/items?itemName=aefly.lumen   <--- ++hot++
- https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-monokai-night

- https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css

- https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens

- https://marketplace.visualstudio.com/items?itemName=tonybaloney.vscode-pets

- https://marketplace.visualstudio.com/items?itemName=vikas.code-navigation
```shell
ext install ms-kubernetes-tools.vscode-kubernetes-tools usernamehw.errorlens s-nlf-fh.glassit MeshIntelligentTechnologiesInc.pieces-vscode miguelsolorio.fluent-icons miguelsolorio.symbols BrandonKirbyson.vscode-animation ryu1kn.partial-diff mikestead.dotenv shalldie.background dbaeumer.vscode-eslint abiospampinato.vscode-monokai-night be5invis.vscode-custom-css eamodio.gitlens tonybaloney.vscode-pets vikas.code-navigation vitest.explorer csstools.postcss ms-playwright.playwright
```






<br><br>
<br><br>
<br><br>
<br><br>


## All
```shell
ext install fabiospampinato.vscode-terminals DanielSanMedium.dscodegpt ryu1kn.partial-diff mikestead.dotenv traBpUkciP.vscode-npm-scripts shalldie.background dbaeumer.vscode-eslint abiospampinato.vscode-monokai-night hoovercj.vscode-power-mode be5invis.vscode-custom-css eamodio.gitlens TabNine.tabnine-vscode tonybaloney.vscode-pets ms-azuretools.vscode-docker TheCodemonkey.synthwave-x-fluoromachine-epic-animations stevencl.addDocComments vikas.code-navigation stevencl.addDocComments gencay.vscode-chatgpt ms-vscode.live-server leodevbro.blockman usernamehw.errorlens s-nlf-fh.glassit ChakrounAnas.turbo-console-log BrandonKirbyson.vscode-animations miguelsolorio.fluent-icons miguelsolorio.symbols rangav.vscode-thunder-client MeshIntelligentTechnologiesInc.pieces-vscode
```


<br><br>
- https://marketplace.visualstudio.com/items?itemName=leodevbro.blockman
- https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server
- https://marketplace.visualstudio.com/items?itemName=ChakrounAnas.turbo-console-log
- https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client

- https://marketplace.visualstudio.com/items?itemName=oouo-diogo-perdigao.docthis
- https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv
  
- https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-power-mode
  
- https://marketplace.visualstudio.com/items?itemName=TabNine.tabnine-vscode
  
- https://marketplace.visualstudio.com/items?itemName=tonybaloney.vscode-pets
  
- https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker
 
  
- https://marketplace.visualstudio.com/items?itemName=gencay.vscode-chatgpt
- 
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
__________________________________________________________________
__________________________________________________________________
<br><br>
<br><br>

# Keybindings
- Open File > Preferences > Keyboard Shortcuts





<br><br>

# Toggle Line Comment

Um den Tastenkürzel in **VSCode** zu ändern, kannst du die folgenden Schritte befolgen:

1. Öffne **VSCode**.
2. Gehe zu den **Einstellungen** (du kannst `Ctrl + ,` verwenden).
3. Suche nach **"Keyboard Shortcuts"** oder gehe direkt zu den **Tastenkombinationen**.
4. Suche nach dem Befehl **"Toggle Line Comment"**.
5. Klicke auf das **Stift-Symbol** neben dem Befehl, um den Tastenkürzel zu ändern.
6. Gib den gewünschten **Tastenkürzel** ein.

Auf diese Weise kannst du den **Tastenkürzel** für das Auskommentieren von Code in **VSCode** anpassen.




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

## Legends Theme (not maintained anymore)
- https://github.com/CyberT33N/vs-code-legends-theme






















<br><br>
<br><br>

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

### Linux
- CTRL + SHIFT + /


### Windows
Öffne die Tastenkombinationen (CTRL + K, dann CTRL + S).
Suche nach "Toggle Line Comment".
Klicke auf den Eintrag und weise CTRL + SHIFT + / als neue Kombination zu.



































<br><br>
<br><br>
__________________________________________________________
__________________________________________________________
<br><br>
<br><br>


# FAQ

## npm not found
First go Settings > search for `package manager` and choose `npm`

1. On your VsCode in Mac : shift + command + P .
2. On the Prompt > type : Terminal: Select Default Profile , then "Click it". Note, as you type you will find this option in the auto-complete .
3. Click the option for zsh or your desired shell.
4. Restart VSCode
