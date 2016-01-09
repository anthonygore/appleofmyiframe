AppleOfMyIframe
===============

Fork that supports jQuery v1.12.0 and adds/modifies a few methods.

Needs a `bower install` to use.

Original project: http://github.com/premasagar/appleofmyiframe

Added methods
-------------

`headScript(content, [,attributes], [,replace])`

Puts a script tag into the head of the iframe document  

**content**  
Type: string  
Content to be inserted into `script` tag  

**attributes**  
Type: object  
Key/value pairs of attributes to be added to script tag e.g. `{type:"text/javascript"}`.

**replace**  
Type: boolean  
Indicates if the script being added should replace any previously added script in the head. False by default.  

`bodyHtml(content, [,emptyFirst])`

Adds HTML to the iframe body. Similar to the `body` method, but will not empty any `script` tags appended to the body
if you set the `emptyFirst` flag to true. If you set the `emptyFirst` flag to false, or, equivalently, omit it, the 
appended HTML will be added after the existing HTML, but before any `script` tags.

**content**  
Type: string  
Content to be inserted/appended to the iframe body.  

**emptyFirst**  
Type: boolean  
Indicates if the content being added should replace any previously added content. Will leave any `script` tags in the
body untouched. False by default. 

`bodyScript(content, [,attributes], [,replace])`

Appends a script tag as the last child of the iframe body. Works the same as the `script` method, except goes in the body,
 not the head. Also, the `replace` flag will not affect any nodes in the body except `script` nodes (this includes `script`
 nodes not added by this method, so keep that in mind).

Modified methods
----------------

`style(cssText, [,replace])`

**replace**  
Type: boolean  
Indicates if the CSS being added should replace any previously added CSS. False by default.  


