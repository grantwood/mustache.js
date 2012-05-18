## WARNING: This is a dangerous fork of Mustache.js.  
This version of Mustache.js no longer HTML escapes {{variables}}, instead it SQL escapes them.

> Wait what?

I'm using Mustache.js to output large SQL scripts, but HTML 
escaping variables isn't safe for this use and SQL escaping is necessary.

Is this a good idea?  Well, yes and no.  Simply SQL escaping output from 
your data into a Mustache template is no substitute for validating and sanitizing 
any incoming data into your system. Having said that, Mustache was a good choice for me
to generate some large SQL scripts.  While my input data has been sanitized and validated,
I still needed to escape dangerous MYSQL characters, thus this fork.


## for the real Mustache.js see:
[mustache.js](http://github.com/janl/mustache.js) is an implementation of the
[Mustache](http://mustache.github.com/) template system in JavaScript.

