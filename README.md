# curl-js
## What is it?
A way how to download a file.

## How it can be useful for me?
When you need a script for downloading a file by JavaScript. 

## How it works?
Sends a request on a http server. When the response is with the status code 200 or 201, saves it.

## How to configure?
There is no configuration needed.

##How to run?
You can run the script from a code:

``` javascript
var curljs = require("curl-js");

curljs.curl(destination, source, function (err) {
    if (err) {
        return;
    }
    // do some stuff
}); 
```

    - destination - path where to save the downloaded file 
    - source - URL address
    - callback - function which is invoked when the file has been downloaded

## What next?
If you have a problem, write me.

### Download to string
Sometimes you appreciate to have a file content in a string

``` javascript
var curljs = require("curl-js");

curljs.curlToString(destination, source, (function (err, content) {
    if (err) {
        return;    
    }
    // do some stuff
}); 
```

    - source - URL address
    - callback - function which is invoked when the file has been downloaded