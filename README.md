# Swiper-3D-Flow

3D Flow plugin for Swiper

3D Flow is the ultra small (1Kb minified and gzipped) and free plugin for iDangero.us Swiper that turns your great swiper slider (or app) into amazing realistic 3D gallery with dynamic shadows. It was inspired by iOS App Store homepage 3D slider.

It works in all browser that support CSS3 3D Transforms: WebKit browsers (Chrome, Safari, iOS Safari, native Android & BlackBerry browsers, etc.), FireFox 12+ and Internet Explorer 10 (including Windows Phone 8). In browsers that do not support CSS3 3D transforms it will work and look like a usual Swiper.

Demos and usage at http://www.idangero.us/sliders/swiper/plugins/3dflow.php

## Note

UMD and non UMD versions are provided.

## Build

This project uses `grunt` to build a dist version.

First you need to have `grunt-cli` which you should install globally.
```
$ npm install -g grunt-cli

```

Then install all dependencies,

```
$ npm install
$ grunt
```

The results is available in `dist` folder.


## Build all versions

To create all versions you can use the `dist` task :
```
$ grunt dist
```

This task is equivalent to :
```
$ grunt build          # the non module version
$ grunt build-umd      # the module compatible version
$ grunt uglify         # minify umd and non umd versions
```
## Demos

### Build

To update demos dependencies you will need to do this first,
```
$ grunt demo
$ cd demos
$ bower install
```


### Launch demos

You can use `npm` `serve` module which will create a temporary local server, that will help you watch the demos with no setup overhead.

If you don't have already `serve` module installed, the recommanded way is to install it globally:
```
$ npm install -g serve
```

Then launch the temporary web server on any port you want, default being 3000, and give the demo path as the root directory.

If you want to launch on port 5000, being in `./demos` folder, type this:
```
$ serve . -p 5000

```

or being in the root folder:
```
$ serve ./demos/ -p 5000
```

You can now point your brower to `http://localhost:5000/`.


## License

GPL & MIT
