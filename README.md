**This starter was for ionic-angular 3.X. I now recommend using the official [Ionic PWA Toolkit](https://github.com/ionic-team/ionic-pwa-toolkit).**

# ionic-starter-pwa

This is a starter template for [Ionic](http://ionicframework.com/docs/) PWA projects.

It is based on the [blank starter](https://github.com/ionic-team/ionic2-starter-blank) with some changes:

* `index.html`
    * activate `service-worker.js`
    * remove `cordova.js`
    * set `maximum-scale=5.0` and remove `user-scalable=no`
    * add a `<noscript>` tag
    * use `<link href="build/FILENAME" rel="preload" as="TYPE">` to preload files (borrowed from https://github.com/shprink/ionic-angular-twitter-pwa)
* `manifest.json`
    * add an icon to `assets/icon` and point to it in `manifest.json`
* `app.components.ts`
    * wrap cordova code with `platform.is('cordova')`
* `variables.scss`
    * remove unused colors from `$colors` (reduces `main.css` file size)

### Building the PWA
```
ionic build --prod
```

### Test it

https://ionic-starter-pwa.firebaseapp.com/

