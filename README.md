![# pynote.js](https://raw.githubusercontent.com/pynote/getpynote/refs/heads/main/pynote.png)

Website : [www.getpynote.net](https://getpynote.net)

**Embed, edit and run Python code and Jupyter Notebooks directly in any HTML page**

To use Pynote, simply add
```html
<script type="module" src="https://cdn.jsdelivr.net/gh/pynote/getpynote/pynote.js"></script>
```

inside the <head> section like this:

```html
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>HTML & Python / Notebook</title>
<script type="module" src="https://cdn.jsdelivr.net/gh/pynote/getpynote/pynote.js"></script>
</head>
<body>

<pynote>
name = 'pynote'
print(name)
</pynote>

</body>
</html>
```

and write your <pynote> tags as shown below.

You can add one or more Pynote tags (same type or different types) in a single HTML page.

### PYNOTE TAGS

**Empty Python editor** - [demo](https://getpynote.net/demo-1.html)
```html
<pynote></pynote>
```

**Editor + code** - [demo](https://getpynote.net/demo-2.html)
```html
<pynote>
name = 'pynote'
print(name)
</pynote>
```

**Editor + Python file** (.py file, either a file hosted on the server or a file loaded from a URL) - [demo](https://getpynote.net/demo-3.html)
```html
<pynote src="https://domain.net/code.py"></pynote>
```

**Jupyter Notebooks** (with editors) (.ipynb file, either a file hosted on the server or a file loaded from a URL) - [demo](https://getpynote.net/demo-4.html)
```html
<pynote src="https://domain.net/notebook.ipynb"></pynote>
```

### OPTIONS
```html
<pynote src="https://domain.net/notebook.ipynb" packages="requests" files="" readonly="true" ></pynote>
```
* `packages` : list of packages to install (names separated by commas) - [demo](https://getpynote.net/demo-5.html)
* `files` : URLs to be added to the Python filesystem for import or manipulation (comma-separated) - [demo](https://getpynote.net/demo-6.html)
* `readonly` : read-only editor (false by default) - [demo](https://getpynote.net/demo-7.html)
