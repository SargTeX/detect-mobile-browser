  [![Build][build-image]][build-url]
  [![NPM Version][npm-image]][npm-url]
  [![NPM Downloads][downloads-image]][downloads-url]
  [![Inline docs][docs-image]][docs-url]
  [![Coverage Status](https://coveralls.io/repos/smali-kazmi/detect-mobile-browser/badge.svg?branch=master&service=github)](https://coveralls.io/github/smali-kazmi/detect-mobile-browser?branch=master)  
  [![NPM][npm-download-image]][npm-url]

Detect Mobile Browser
=====================

Small plugin to detect mobile browser 

**Usage Frotnend:-**

```javascript
alert(SmartPhone.isAndriod());
```

OR

```javascript
alert(SmartPhone.isAny());
```

**Usage Backend:-**

User as a ExpressJS middleware

```javascript
var mobileBrowser = require('./detect-browser');

...
...

app.use(mobileBrowser());

app.get('/', function (req, res){
    ...
    ...
    //in req
    console.log(req.SmartPhone.isAny());

    ...
    ...

    //in res locals to use in templates
    console.log(res.locals.SmartPhone.isAny());

    ...
    ...

});

```



## Bower

    $ bower install browser-detector --save

## NPM

    $ npm install detect-mobile-browser --save

[npm-image]: https://img.shields.io/npm/v/detect-mobile-browser.svg
[npm-download-image]: https://nodei.co/npm/detect-mobile-browser.png?downloads=true&downloadRank=true
[npm-url]: https://www.npmjs.com/package/detect-mobile-browser
[downloads-image]: https://img.shields.io/npm/dm/detect-mobile-browser.svg
[downloads-url]: https://www.npmjs.com/package/detect-mobile-browser
[docs-image]: http://inch-ci.org/github/smali-kazmi/detect-mobile-browser.svg?branch=master
[docs-url]: http://inch-ci.org/github/smali-kazmi/detect-mobile-browser
[build-image]: https://api.travis-ci.org/smali-kazmi/detect-mobile-browser.svg?branch=master
[build-url]: https://travis-ci.org/smali-kazmi/detect-mobile-browser