---
id: option-unformatted
title: Unformatted
sidebar_label: ✅ Unformatted
---
**Key**: `unformatted`

**Description**: List of tags (defaults to inline) that should not be reformatted

**Type**: `array of strings`

**Default**: `["a","abbr","area","audio","b","bdi","bdo","br","button","canvas","cite","code","data","datalist","del","dfn","em","embed","i","iframe","img","input","ins","kbd","keygen","label","map","mark","math","meter","noscript","object","output","progress","q","ruby","s","samp","select","small","span","strong","sub","sup","svg","template","textarea","time","u","var","video","wbr","text","acronym","address","big","dt","ins","small","strike","tt","pre","h1","h2","h3","h4","h5","h6"]`

## Support
**Languages**: [HTML](/docs/language-html.html), [Handlebars](/docs/language-handlebars.html), [Liquid](/docs/language-liquid.html), [Mustache](/docs/language-mustache.html), [XML](/docs/language-xml.html)

**Beautifiers**: [JS-Beautify](/docs/beautifier-js-beautify.html)

<details><summary><strong>Comparison Table</strong></summary>
| Language | [JS-Beautify](/docs/beautifier-js-beautify.html) |
| --- | --- |
| [HTML](/docs/language-html.html) | &#9989; |
| [Handlebars](/docs/language-handlebars.html) | &#9989; |
| [Liquid](/docs/language-liquid.html) | &#9989; |
| [Mustache](/docs/language-mustache.html) | &#9989; |
| [XML](/docs/language-xml.html) | &#9989; |
</details>
## Examples
### HTML
<details><summary><strong>🚧 Original Code</strong></summary>
```HTML
<div>
<h1>Unformatted</h1>
<div>
<span>Un<span>formatted</span></span>
</div>
<span><span>For</span><span>mat</span><span>ted</span></span>
<div><div>For</div><div>mat</div><div>ted</div></div>
</div>

```
</details>
<details><summary><strong>🔧 `[]`</strong></summary>
Using [JS-Beautify](/docs/beautifier-js-beautify.html) beautifier:
```HTML
<div>
  <h1>Unformatted</h1>
  <div>
    <span>Un
      <span>formatted</span>
    </span>
  </div>
  <span>
    <span>For</span>
    <span>mat</span>
    <span>ted</span>
  </span>
  <div>
    <div>For</div>
    <div>mat</div>
    <div>ted</div>
  </div>
</div>
```
<details><summary>Configuration</summary>
A `.unibeautify.json` file would look like the following:
```json
{
  "HTML": {
    "indent_size": 2,
    "indent_char": " ",
    "unformatted": []
  }
}
```
</details>
<details><summary>Difference from original</summary>
```diff
Index: 
===================================================================
--- 	Original
+++ 	Beautified
@@ -1,8 +1,18 @@
 <div>␊
-<h1>Unformatted</h1>␊
-<div>␊
-<span>Un<span>formatted</span></span>␊
-</div>␊
-<span><span>For</span><span>mat</span><span>ted</span></span>␊
-<div><div>For</div><div>mat</div><div>ted</div></div>␊
-</div>␊
+␣␣<h1>Unformatted</h1>␊
+␣␣<div>␊
+␣␣␣␣<span>Un␊
+␣␣␣␣␣␣<span>formatted</span>␊
+␣␣␣␣</span>␊
+␣␣</div>␊
+␣␣<span>␊
+␣␣␣␣<span>For</span>␊
+␣␣␣␣<span>mat</span>␊
+␣␣␣␣<span>ted</span>␊
+␣␣</span>␊
+␣␣<div>␊
+␣␣␣␣<div>For</div>␊
+␣␣␣␣<div>mat</div>␊
+␣␣␣␣<div>ted</div>␊
+␣␣</div>␊
+</div>
\ No newline at end of file

```
</details>
</details>
<details><summary><strong>🔧 `["a","abbr","area","audio","b","bdi","bdo","br","button","canvas","cite","code","data","datalist","del","dfn","em","embed","i","iframe","img","input","ins","kbd","keygen","label","map","mark","math","meter","noscript","object","output","progress","q","ruby","s","samp","select","small","span","strong","sub","sup","svg","template","textarea","time","u","var","video","wbr","text","acronym","address","big","dt","ins","small","strike","tt","pre","h1","h2","h3","h4","h5","h6"]`</strong></summary>
Using [JS-Beautify](/docs/beautifier-js-beautify.html) beautifier:
```HTML
<div>
  <h1>Unformatted</h1>
  <div>
    <span>Un<span>formatted</span></span>
  </div>
  <span><span>For</span><span>mat</span><span>ted</span></span>
  <div>
    <div>For</div>
    <div>mat</div>
    <div>ted</div>
  </div>
</div>
```
<details><summary>Configuration</summary>
A `.unibeautify.json` file would look like the following:
```json
{
  "HTML": {
    "indent_size": 2,
    "indent_char": " ",
    "unformatted": [
      "a",
      "abbr",
      "area",
      "audio",
      "b",
      "bdi",
      "bdo",
      "br",
      "button",
      "canvas",
      "cite",
      "code",
      "data",
      "datalist",
      "del",
      "dfn",
      "em",
      "embed",
      "i",
      "iframe",
      "img",
      "input",
      "ins",
      "kbd",
      "keygen",
      "label",
      "map",
      "mark",
      "math",
      "meter",
      "noscript",
      "object",
      "output",
      "progress",
      "q",
      "ruby",
      "s",
      "samp",
      "select",
      "small",
      "span",
      "strong",
      "sub",
      "sup",
      "svg",
      "template",
      "textarea",
      "time",
      "u",
      "var",
      "video",
      "wbr",
      "text",
      "acronym",
      "address",
      "big",
      "dt",
      "ins",
      "small",
      "strike",
      "tt",
      "pre",
      "h1",
      "h2",
      "h3",
      "h4",
      "h5",
      "h6"
    ]
  }
}
```
</details>
<details><summary>Difference from original</summary>
```diff
Index: a,abbr,area,audio,b,bdi,bdo,br,button,canvas,cite,code,data,datalist,del,dfn,em,embed,i,iframe,img,input,ins,kbd,keygen,label,map,mark,math,meter,noscript,object,output,progress,q,ruby,s,samp,select,small,span,strong,sub,sup,svg,template,textarea,time,u,var,video,wbr,text,acronym,address,big,dt,ins,small,strike,tt,pre,h1,h2,h3,h4,h5,h6
===================================================================
--- a,abbr,area,audio,b,bdi,bdo,br,button,canvas,cite,code,data,datalist,del,dfn,em,embed,i,iframe,img,input,ins,kbd,keygen,label,map,mark,math,meter,noscript,object,output,progress,q,ruby,s,samp,select,small,span,strong,sub,sup,svg,template,textarea,time,u,var,video,wbr,text,acronym,address,big,dt,ins,small,strike,tt,pre,h1,h2,h3,h4,h5,h6	Original
+++ a,abbr,area,audio,b,bdi,bdo,br,button,canvas,cite,code,data,datalist,del,dfn,em,embed,i,iframe,img,input,ins,kbd,keygen,label,map,mark,math,meter,noscript,object,output,progress,q,ruby,s,samp,select,small,span,strong,sub,sup,svg,template,textarea,time,u,var,video,wbr,text,acronym,address,big,dt,ins,small,strike,tt,pre,h1,h2,h3,h4,h5,h6	Beautified
@@ -1,8 +1,12 @@
 <div>␊
-<h1>Unformatted</h1>␊
-<div>␊
-<span>Un<span>formatted</span></span>␊
-</div>␊
-<span><span>For</span><span>mat</span><span>ted</span></span>␊
-<div><div>For</div><div>mat</div><div>ted</div></div>␊
-</div>␊
+␣␣<h1>Unformatted</h1>␊
+␣␣<div>␊
+␣␣␣␣<span>Un<span>formatted</span></span>␊
+␣␣</div>␊
+␣␣<span><span>For</span><span>mat</span><span>ted</span></span>␊
+␣␣<div>␊
+␣␣␣␣<div>For</div>␊
+␣␣␣␣<div>mat</div>␊
+␣␣␣␣<div>ted</div>␊
+␣␣</div>␊
+</div>
\ No newline at end of file

```
</details>
</details>