# Third party libs

## best

browser based jquery
```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Learning TypeScript</title>
    <script src="node_modules/systemjs/dist/system.js"></script>
</head>
<body>
<div id="app">Change it with jQuery</div>
<script>
    // set our baseURL reference path
    SystemJS.config({
        map: {
            "jQuery": "node_modules/jquery/dist/jquery.min.js"
        },
        baseURL: '/',
        defaultJSExtensions: true
    });
    SystemJS.import('app.js');
</script>
</body>
</html>
```

type support gotten with `npm install @types/jquery`

## weak

created own type file `jquery.d.ts`

```
const declare $:any;
```
