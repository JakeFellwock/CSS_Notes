STYLE Attribute
The ```<style> ```tag is used to define style information (CSS) for a document. <br>
Inside the ```<style>``` element you specify how HTML elements should render in a browser. <br>
The ```<style>``` element must be included inside the ```<head>``` section of the document. <br>
 ```<style>``` <br>
 ```   h1 {text-align: center;}``` <br>
 ```</style>``` <br>
```
   <style>
      h1 { 
       text-align: center;
       }
      h2 {
       text-align: center;
     }
      p {
       text-align: center;
      }
      
   </style>
```


You can separate selectors by "," to add multiple elements to the same style sheet
```
   <style>
    h1, h2, p {
     text-align: center;
     }
   </style>
```

You have styled three elements by writing CSS inside the style tags. This works, but since there will be many more styles, it's best to put all the styles in a separate file and link to it. <br>

Create a separate styles.css file and add it to the project directory. <br>

Now you need to link the styles.css file so the styles will be applied. Nest a self-closing link element in the head element<br> Give it a rel attribute value stylesheet and an href attribute value of styles.css. <br>
```
    <head>
      <link rel="stylesheet" href="styles.css"
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
    </head>
```
Comments in CSS look like this: <br>
```/* comment here */ <br>```

So far you have been using type and id selectors to style elements. However, it is more common to use a different selector to style your elements. <br>

A class selector is defined by a name with a dot directly in front of it, like this:<br>
```
.class-name {
  styles
}
```

Change the existing #menu selector into a class selector by replacing #menu with a class named .menu. <br>

You can use an hr element to display a divider between sections of different content. <br>
self closing ``<hr>`` inserts a line  <br>


Example CSS: 
```
body {
  background-image: url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg);
  font-family: sans-serif;
  padding: 20px;
}

h1 {
  font-size: 40px;
  margin-top: 0;
  margin-bottom: 15px;
}

h2 {
  font-size: 30px;
}

.established {
  font-style: italic;
}

h1, h2, p {
  text-align: center;
}

.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
  padding: 20px;
  max-width: 500px;
}
hr {
  height: 2px;
  background-color: brown;
  border-color: brown;
}

.bottom-line {
  margin-top: 25px;
}

h1, h2 {
  font-family: Impact, serif;
}

.item p {
  display: inline-block;
  margin-top: 5px;
  margin-bottom: 5px;
  font-size: 18px;
}

.flavor, .dessert {
  text-align: left;
  width: 75%;
}

.price {
  text-align: right;
  width: 25%;
}

/* FOOTER */

footer {
  font-size: 14px;
}

.address {
  margin-bottom: 5px;
}

a {
  color: black;
}

a:visited {
  color: black;
}

a:hover {
  color: brown;
}

a:active {
  color: brown;
}
```
