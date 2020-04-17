# TilejsonTester
Web Interface for creating and testing tilejson files

Try it at [http://trailbehind.github.io/TilejsonTester/](http://trailbehind.github.io/TilejsonTester/)

It imports tiles from the URL you specify, and displays the results on a map, so you can judge if it will display properly.

The tester does some sanity checking on the bounds (the west bound must be less than the east, and the south must be less than the north.) 
In addition, the tester draws a rectangle around the bounds on the map so you can be sure that all tiles are entirely included.

## To work on this app...

It's straightforward to develop this app further on your local machine. 
The process uses [browser-sync](https://browsersync.io/#install). 
The command below installs `browser-sync` on your computer. 
Installing it globally (with "-g") means that you can use it in many different projects, 
so you only need to do it once.

```
npm install -g browser-sync		
```

Next, clone the git repository to your local disk. Then `cd` to the repository's directory, and run `browser-sync`.

It starts a local web server, finds the `index.html` file, and displays it in your browser. 
When you save changes to files, 
it automatically updates the browser window. To use it:

```
git clone https://github.com/trailbehind/TilejsonTester.git

cd TilejsonTester

browser-sync start --server --files "*.html"
```
