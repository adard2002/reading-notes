# Reading 11 Notes

[Home](README.md)
# EJS
## What is EJS?
It's a templating language that generates HTML markup with JavaScript. It does look a lot like a normal HTML file but it does have some different code we have not used yet. Instead of using an HTML file for HTML that will show up on your page it shows on plain JS pretty much kinda maybe.


## EJS Tutorial WalThroughCode 
- Install --save express, body-parser, and cors and ejs
- Will usually use 8000 or 8080 for EJS
- 
## Injecting values into the views
To get these to render in the main index page you are going to want the following code in your server.js:

var express = require('express');<br>
var bodyParser = require('body-parser');<br>
var cors = require('cors');<br>
var path = require('path');<br>

var app = express();<br>

app.use(bodyParser());<br>
app.use(cors());<br>

app.set('views', path.join(_dirname, 'views'));<br>
app.set('view engine', 'ejs');<br>

app.get('/', function(request, response) {<br>
  response. render('index', {<br>
    foo: 'bar'<br>
  });<br>
});<br>

app.listen(8000, function() {
  console.log("heard on 8000");
});


### Using EJS in HTML elements
- An example of using an EJS is:
&lt;h1&gt;Hello &lt;%= foo %&gt;&lt;/h1&gt; the = sign says we are going to evaluate a variable.

- Can use in img tags too:
&lt;img src="&lt;%= foo %&gt;" alt=""&gt;

- Can be used in anchor tags:
&lt;a href="/&lt;%= foo.id %&gt;/destroy"&gt;&lt;/a&gt;

### For loops and Arrays
To write an array all you need to change in your server.js file will be the app.get('/') function: 

app.get('/', function(request, response) {<br>
  response. render('index', {<br>
    people: [<br>
    { name: 'Dave' },<br>
    { name: 'Jerry' }<br>
    ]<br>
  });<br>
});<br>

After you have the previous code in your server.js you are going to want to put this in your index.ejs:
&lt;ul&gt; <br>
&lt;% for (var person of people) { %&gt; <br>
&lt;li&gt;&lt;%= person.name %&gt;&lt;/li&gt; <br>
&lt;% } %&gt; <br>
&lt;/ul&gt; <br>

This will return the names Dave and Jerry in an unordered list

### If/Else statement
In the code below we are saying if their name is Dave then they are definitely dave. You are NOT going to need an = sign since we are only writing an if statement. No evaluating anything.

&lt;ul&gt; <br>
    &lt;% for (var person of people) { %&gt; <br>
      &lt;% if(person.name === 'Dave') { %&gt; <br>
      &lt;li&gt;This is definitely &lt;%= person.name %&gt;!!!!&lt;/li&gt; <br>
        &lt;% } else { %&gt; <br>
          &lt;&gt;This is definitely not Dave!!! This is &lt;%= person.name %&gt;&lt;/li&gt; <br>
      &lt;% } %&gt; <br>
  &lt;% } %&gt; <br>
&lt;/ul&gt; <br>