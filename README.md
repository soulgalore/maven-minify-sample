# Example project minifying js & css with Maven

This is a working pom.xml file using the maven-minify-plugin, gziping the result and replacing the current css/js 
links in configured files to the minified version.

## This is what happens

1. Creates one css file from existing css-files
2. Creates one js file from existing js-files
3. Minifies them
4. Give the minified js and css files unique names for each release (right now using time stamp)
5. Creates gzipped versions

## How to use it
```
mvn clean package
```

## What you need to do
Configure your web server to pick the gz-versions of the files.


## Structure of the project
The /src/-tree holds an example setup with two css & two js files that are concated & minified and example files 
that hold references/links to the actual js/css files.


## TODO
The naming of the css/js file uses the current date/time, not so good if you releasing multiple times a day, needs to be changed!