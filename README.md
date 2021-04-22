# jsfile
JavaScript file packager
# Usage
To make a  JSfile instance, use this script:

```javascript
var maker=new JSfile();
```

To edit the content of the file, use this:
```javascript
maker.setContent('Hello World!');
```

To set the MIME type, use this:

```javascript
maker.setMimeType('text/plain');
```

And finally, to get the file (as a blob), use this:

```javascript 
maker.getFile();
```

A way you can use ```getFile();``` would be this:

```javascript
var a=document.querySelector('a');
a.href=maker.getFile();
a.download="download";
```
