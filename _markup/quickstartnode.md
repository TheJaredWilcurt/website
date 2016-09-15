Create `index.html`:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hello World!</title>
  </head>
  <body>
    We are using node.js <script>document.write(process.version)</script>.
    <script> nw.Window.get().showDevTools(); </script>
  </body>
</html>
```

Create `package.json`:

```json
{
    "name": "your_application_name",
    "main": "index.html",
    "devDependencies": { "nw": "0.14.7-sdk" },
    "scripts": { "start": "nw ." }
}
```

Then just run:

1. `npm install`
2. `npm start`

And it will automatically launch NW.js and open your `index.html` file that is located next to your `package.json` file.

* * *

For a more fleshed out version of an NW.js `package.json` file, see this example from [UGUI](http://UGUI.io) (an NW.js framework):

* [UGUI package.json](http://ugui.io/package)
