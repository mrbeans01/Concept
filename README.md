# Concept
Basic Concept
<pre>

# Javascript Objects and functions
## FUNCTIONS AS FIRST-CLASS OBJECTS

Objects in JavaScript enjoy certain capabilities:

 They can be created via literals.
 
 They can be assigned to variables, array entries, and properties of other objects.
 
 They can be passed as arguments to functions.
 
 They can be returned as values from functions.
 
 They can possess properties that can be dynamically created and assigned
 

>> Functions in JavaScript possess all of these capabilities and are thus treated like any
other object in the language. Therefore, we say that they’re first-class objects.
And more than being treated with the same respect as other object types, functions
have a special capability in that they can be invoked



Scoping and functions

Variable declarations are in scope from their point of declaration to the end of
the function within which they’re declared, regardless of block nesting.

Named functions are in scope within the entire function within which they’re
declared, regardless of block nesting. (Some call this mechanism hoisting.)

For the purposes of declaration scopes, the global context acts like one big
function encompassing the code on the page.


 Invocations
 

There are actually four different ways to invoke a function, each with its
own nuances:

As a function, in which the function is invoked in a straightforward manner

As a method, which ties the invocation to an object, enabling object-oriented
programming

As a constructor, in which a new object is brought into being

Via its apply() or call() methods, which is kind of complicated, so we’ll cover
that when we get to it



Invocation as a constructor


Invoking a function as a constructor is a powerful feature of JavaScript, because when
a constructor is invoked, the following special actions take place:

A new empty object is created.

This object is passed to the constructor as the this parameter, and thus
becomes the constructor’s function context.

In the absence of any explicit return value, the new object is returned as the
constructor’s value.

function Ninja() {
this.skulk = function() { return this; };
}
var ninja1 = new Ninja();
var ninja2 = new Ninja();



Functions are first-class objects that are treated just like any other objects within
JavaScript. Just like any other object type, they can be:
– Created via literals
– Assigned to variables or properties
– Passed as parameters
– Returned as function results
– Possess properties and methods


Each object has a “super power” that distinguishes it from the rest; for functions
it’s the ability to be invoked.

Functions are created via literals, for which a name is optional.

The browser can invoke functions during the lifetime of a page by invoking
them as event handlers of various types.

The scope of declaration within a function differs from that of most other languages.
Specifically:
– Variables within a function are in scope from their point of declaration to
the end of the function, spanning block boundaries.
– Inner named functions are available anywhere within the enclosing function
(hoisted), even as forward references.
■ The parameter list of a function and its actual argument list can be of different
lengths:
– Unassigned parameters evaluate as undefined.
– Extra arguments are simply not bound to parameter names.
■ Each function invocation is passed two implicit parameters:
– arguments, a collection of the actual passed arguments
– this, a reference to the object serving as the function context
■ Functions can be invoked in various ways, and the invocation mechanism determines
the function context value:
– When invoked as a simple function, the context is the global object (window).
– When invoked as a method, the context is the object owning the method.
– When invoked as a constructor, the context is a newly allocated object.
– When invoked via the apply() or call() methods of the function, the context
can be whatever the heck we want.

Anonymous functions can be named but those names are only visible within the functions themselves.
var ninja = {  
yell: function yell(n){    return n > 0 ? yell(n-1) + "a" : "hiy";  }
 }; 
assert( ninja.yell(4) == "hiyaaaa",  "Works as we would expect it to!" );
var samurai = { yell: ninja.yell };
 var ninja = {};
 assert( samurai.yell(4) == "hiyaaaa",  "The method correctly calls itself." );// this will pass 


Function Length
. This property equates to the number of arguments that the function is expecting. 




# JavaScript magics





AJAX Asynchronous  Javascript and xml  

if (window.XMLHttpRequest) { // Mozilla, Safari, IE7+ ...
    httpRequest = new XMLHttpRequest();
} else if (window.ActiveXObject) { // IE 6 and older
    httpRequest = new ActiveXObject("Microsoft.XMLHTTP");
}

https://developer.mozilla.org/en-US/docs/AJAX/Getting_Started


The full list of the readyState values is documented at XMLHTTPRequest.readyState and is as follows

0 (uninitialized) or (request not initialized)
1 (loading) or (server connection established)
2 (loaded) or (request received)
3 (interactive) or (processing request)
4 (complete) or (request finished and response is ready)


>> Clousre
<pre>
var add = (function () {
    var counter = 0;
    return function () {return counter += 1;}
})();
</pre>
>> Currying 
<pre>
var add = function(a){
	return function(b){
	return a+b;
	}
}
</pre>

Promises and callback


REST API 
Representational state transfer (REST) or RESTful Web services are one way of providing interoperability between computer systems on the Internet


rest vs soap web services
http/s   others
can use any format     XML  



Higher order fucntion :- callbacks



WebSockets()







Capability to design / use frameworks for responsive front applications interacting

with backend Restful web services. Must be familiar with Angular.JS, HTML5, CSS3.

Must be very strong in Javascript and know how to craft the language to generate JS

Objects based off design patterns like Singleton, Factory, etc. Must know

WebSockets; Must know how to work with Asynchronous services. Must know how

to handle pull/request based and push/event based, data. Must know diverse

widget toolkits like Kendo, JQuery, ExtJS, Dojo, etc. Must know something of TDD

and create detailed wire frames &amp; process flows. Must be able to rapidly test these

UI artifacts. Must be able to write various methods to manipulate HTML, CSS in

Jquery or other JS toolkits, as well as making the pages dynamic using AJAX, JSON

and XML. Must know the underlying model behind AJAX. Must know how to resolve

Browser compatibilty issues.

Familiarity with containers like Docker a plus; Some familiarity with tomcat, jetty or

nginx a plus; Familiarity with Web/REST applications a plus.


</pre>
