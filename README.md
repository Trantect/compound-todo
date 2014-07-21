### Welcome to CompoundJS ###

This is a demo TODO project with CompoundJS, Jade, CoffeeScript and LESS.

#### How to run it ####

```
npm install
coffee server.coffee
```

#### How was it created ####

##### Install CompoundJS #####

```
npm install compound -g
```

##### Initialize the project with Jade and CoffeeScript #####

```
compound init compound-todo --tpl jade --coffee --css less
cd compound-todo
npm install
```

##### Create a CRUD with Jade and CoffeeScript #####

```
compound generate crud post title content date:date published:boolean --tpl jade --coffee

```
model name must define less letter，else you will get undefine error
##### Correct doctype #####

CompoundJS generated .jade files with a old style. So, you will need to correct the .jade files by replacing _!!! 5_ with _doctype html_.

##### Error: Cannot find module 'jade~' #####

You may get this error message after editing a .jade file. Just find the .jade~ file and delete it.
