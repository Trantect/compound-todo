### Welcome to CompoundJS ###

This is a demo TODO project with CompoundJS, Jade and CoffeeScript.

#### How was it created ####

##### Install CompoundJS #####

```
npm install compound -g
```

##### Initialize the project with Jade and CoffeeScript #####

```
compound init compound-todo --tpl jade --coffee
cd compound-todo
npm install
```

##### Create a CRUD with Jade and CoffeeScript #####

```
compound generate crud post title content date:date published:boolean --tpl jade --coffee
```

##### Correct doctype #####

CompoundJS generated .jade files with a old style. So, you will need to correct the .jade files by replacing **!!! 5** with **doctype html**.

##### Error: Cannot find module 'jade~' #####

You may get this error message after editing a .jade file. Just find the .jade~ file and delete it.
