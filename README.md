# **PowerMill Macro Syntax Highlight for VSCode**

Autodesk's CAM software <b>"PowerMill" </b> has a powerful macro language.

For detailed language specifications, please see [Autodesk PowerMill Macro Programming Guide](https://knowledge.autodesk.com/sites/default/files/file_downloads/PM-Macro_Programming_Guide.pdf).


If you wish to develop with .NET, please use here.
['PowerShape and PowerMill API'](https://github.com/Autodesk/PowerShapeAndPowerMillAPI)


## Installation 
- Install the 'PowerMillMacro-x.x.x.vsix' file into VSCode.

## Features
+ syntaxes
    + Functions in Powermill 2020 'Parameter Reference'.
    + Language specification control statements.

+ snippets
    + function
    + if , if..else , if..elseif
    + switch
    + foreach
    + while
    + message info

## Known Issues
+ The parameter at the time of function declaration does not syntax highlight correctly.

## License
+ MIT

## Acknowledgments
+ Thank you [everyone in the forum](https://forums.autodesk.com/t5/powermill-forum/bd-p/280).


## 日本語環境で使用する
+ 日本語言語でマクロを作成する際、エンコード "Shift-JIS" にする必要があります。setting.jsonに以下を追記すると便利です。

``` json
    "files.associations": {
        "*.mac": "pmillmacro",
        "*.inc": "pmillmacro"
    },
    "[pmillmacro]": {
        "files.encoding": "shiftjis"
    }
```