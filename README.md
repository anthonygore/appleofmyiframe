AppleOfMyIframe
===============

Fork that supports jQuery v1.12.0

Needs a `bower install` to use.

Original project: http://github.com/premasagar/appleofmyiframe

Added methods
-------------

`script(content, [,attributes], [,replace])`

Puts a script tag into the head of the document  

**content**  
Type: string  
Content to be inserted into `script` tag  

**attributes**  
Type: object  
Key/value pairs of attributes to be added to script tag e.g. `{type:"text/javascript"}`  

**replace**  
Type: boolean  
Indicates if the CSS being added should replace any previously added CSS. False by default.  

Modified methods
----------------

`style(cssText, [,replace])`

**replace**  
Type: boolean  
Indicates if the CSS being added should replace any previously added CSS. False by default.  


