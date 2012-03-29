Example project minifying js & css with maven
=================

This is a working pom.xml file using the maven-minify-plugin, gziping the result and replacing the current css/js 
links to the minified version.

-- This is what happens:

1. Create one css file from existing css-files
2. Create one js file from existing js-files
3. Minify them
4. Give the minified js and css files unique names for each release
5. Gzip them and create gzipped versions


-- What you need to do
Configure your webserver to pick the gz-versions of the files.

-- How to use it:
```
mvn clean package
```
-- The src-tree holds an example setup


-- TODO: the naming of the css/js file uses the current date, not so good if you releasing multiple times a day, needs to be changed