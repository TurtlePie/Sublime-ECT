
Sublime Text 2 Syntax highlighting for ECT, embedded CoffeeScript HTML  
Additionally, as ECT is backward compatible with ECO, so is this.

See: http://ectjs.com

Comes with sets of open and close tags:

```
<% %>
<< >>
<? ?>
{{ }}
```

You would specify `open` and `close` options when you create a new ECT engine/renderer, within your application.

### Install

Via the [Sublime Package Manager](http://wbond.net/sublime_packages/package_control), under `ECT`.  
Or simply clone this repo into `/Sublime Text 2/Data/Packages/ECT/`

### Optional

You may create your own tags by copying a .tmLanguage file.  
The `{{ }}` template, `ect_html3.tmLanguage`, would be the easiest.  

Replace all occurances (they're all contained within one `<dict>` around line `500`) of each open and close tag with your own tags

Also, be sure to rename the .tmLanguage near the top of the file:
```
<key>name</key>
<string>ECT {{</string>
```
Note that html characters must be encoded within the .tmLanguage files. eg. `<` is expressed as `&lt;`

