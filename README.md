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


# Trandy Quest

#TypeScript 

TypeScript is a free and open-source programming language developed and maintained by Microsoft. It is a strict syntactical superset of JavaScript

TypeScript’s main benefits:

	Class and Module Support    , purely oops based
	Static Type-checking
	ES6 Feature Support
	Clear Library API Definition
	Build-in Support for JavaScript Packaging
	Syntax Similarity to Our Backend Languages (Java, Scala)
	Superset of JavaScript



#ES6 Features

Block-Scoped Constructs Let and Const
Arrow Functions in ES6

Default Parameters in ES6
Template Literals in ES6
Multi-line Strings in ES6
Destructuring Assignment in ES6
Enhanced Object Literals in ES6

Promises in ES6
Classes in ES6
Modules in ES6


Diffences Between Angular 2 ,4 Vs Angular 1



scss nesting lavel (4 Max)
https://css-tricks.com/forums/topic/sass-best-practices-nesting-more-than-3-levels-deep/
http://thesassway.com/beginner/the-inception-rule


Hanlde image in different device size  (responsive images)?  
srcSet

https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images

accessebility feature 






# Normalize.css 

  Normalize.css is a small CSS file that provides better cross-browser consistency in the default styling of HTML elements. It's a modern, HTML5-ready, alternative to the traditional CSS reset.


# Cross browser compatibility problems
   common  issues

   1. Incorrect (or no) DOCTYPE
   2. No CSS Reset
      A few commonly used reset style sheets are:
      Normalize.css
      HTML5Reset
      

      Make sure to have one of these added as the first style sheet to your page to ensure a proper CSS reset.

   3. Vendor Specific CSS Styles
      If a browser vendor implements a new CSS functionality they will often hide it behind a so called vendor specific CSS style. 

   4. Lack of Valid HTML / CSS
     Different browsers interpret HTML and CSS differently, and some are more forgiving than others. 

   5. Outdated Browser Detection


 ** more details 
  http://www.airccse.org/journal/ijsea/papers/0711ijsea05.pdf

  https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/HTML_and_CSS



# speed up your site

 * Minimize HTTP Requests
 * Reduce server response time
 * Enable compression
 * Enable browser caching
 * Minify Resources
 * Optimize images 
  With images, you need to focus on three things: size, format and the src attribute.
     Image size
     Image format
        JPEG is your best option.
        PNG is also good, though older browsers may not fully support it.
        GIFs should only be used for small or simple graphics (less than 10×10 pixels, or a color palette of 3 or fewer colors) and for animated images.
        Do not use BMPs or TIFFs.
     Src attribute
        In particular, avoid empty image src codes.
 * Optimize CSS Delivery
   In general, an external style sheet is preferable, because it reduces the size of your code and creates fewer code duplications.
 * Reduce redirects




 Cross domain , cross origin  CORS ??
 
 
 
 
 


What are reflows and repaints and how to avoid them

Its becom­ing increas­ingly com­mon for the topic of reflows and repaints to come up when talk­ing about improv­ing page per­for­mance. Although the two of them are closely related, they dif­fer in terms of the impact each can have on browser performance.

Repaint

A repaint occurs when you change the styling of an ele­ment such that it does not effect its lay­out. For e.g. When you change the back­ground color or out­line etc.

Causes of repaints
In essence, any­thing that causes the visual appear­ance of a DOM node to change causes a repaint of that par­tic­u­lar dom node and more than likely all of its chil­dren. Some of the causes or repaints are

Scrolling: When you scroll, the browser has to redraw the pix­els at the place that you scrolled. This is one is not as eas­ily avoidable.
Chang­ing vis­i­bil­ity or col­ors or back­ground colors.



Reflow

A reflow pri­mar­ily occurs when the lay­out of an ele­ment changes. It causes the browser to recom­pute the dimen­sions and posi­tion­ing of the par­ent and child nodes and some­times even ances­tors and sib­lings. Browser imple­men­ta­tions dif­fer in the way they opti­mize for reflows.

The most impor­tant point to be aware of in this dis­cus­sion is

A reflow is a user-blocking oper­a­tion. It con­sumes rel­a­tively higher CPU time and will result in a degraded user expe­ri­ence on a mobile device if it hap­pens to often.


Causes of reflows
As a rule of thumb — any­thing that affects the cur­rent ‘flow’ of ele­ments in the page will trig­ger a reflow. Some of the causes of reflows are

Resiz­ing the window
Mov­ing your mobile device(tablet/phone) from land­scape to por­trait mode and vice versa.
Chang­ing the font size
Cal­cu­lat­ing off­setWidth and offsetHeight
Chang­ing the height, width, positions
Chang­ing inline styles
Using JavaScript meth­ods involv­ing com­puted styles
Adding/removing ele­ments from the dom

In most cases, reflows are fol­lowed by a repaint.


Ways to min­i­mize reflows and repaints

DOM oper­a­tions involv­ing ani­ma­tions should prefer­able done out of the flow using — posi­tion absolute or fixed.
Change classes at the low­est lev­els in the DOM tree.
Avoid using inline style. Aside from that, not only are they a night­mare to main­tain, they also increase amount of markup to be delivered(if you are doing server side render).
Avoid tables for lay­out. Because the con­tent of any cell in a table can impact the dimen­sions of another cell in the table, it causes mul­ti­ple passes to be ren­dered. There­fore almost any change to a table can cause reflows.
When­ever pos­si­ble if new nodes are to be added to the DOM, batch together oper­a­tions that manip­u­late them before insert­ing them into the DOM.
When read­ing com­puted styles like off­setWidth and off­setHeight, don’t inter­leave them with a write to those prop­er­ties. e.g. If you already retrieved a node.offsetHeight, batch all other such read oper­a­tions until you write to the dom again. Thats because con­sec­u­tive reads on com­puted styles will not trig­ger a reflow.
Debounce the win­dow resize event han­dler, if any.





 // find longest unique sub string lentgh

https://gist.github.com/primaryobjects/3bbf42ed7fdd537cd88705de2edd5120


function maxSubstring(s){
  var max =0;
  var lastIndex =0;
  var arr = [];
  var newStr='';
  for (var i=0; i<s.length ;i++)
  {

   if(arr[s[i]])
   {
        if (newStr.length > max) {  
            max = newStr.length;
        }

        var start = newStr.indexOf(s[i]);
        newStr = newStr.substring(start + 1); 
   }
 	  newStr += s[i];
    arr[s[i]] = i + 1;

  }

  return max;
 
}



# What happens when you type an URL in the browser and press enter ans then?

The browser checks the cache for a DNS record to find the corresponding IP address of maps.google.com.
 In order to find the DNS record, the browser checks four caches.
  1.First, it checks the browser cache. The browser maintains a repository of DNS records for a fixed duration for websites you have previously visited. So, it is the first place to run a DNS query.
  2.Second, the browser checks the OS cache. If it is not found in the browser cache, the browser would make a system call (i.e. gethostname on Windows) to your underlying computer OS to fetch the record since the OS also maintains a cache of DNS records.
  3.Third, it checks the router cache. If it’s not found on your computer, the browser would communicate with the router that maintains its’ own cache of DNS records.
  4.Fourth, it checks the ISP cache. If all steps fail, the browser would move on to the ISP. Your ISP maintains its’ own DNS server which includes a cache of DNS records which the browser would check with the last hope of finding your requested URL.

If the requested URL is not in the cache, ISP’s DNS server initiates a DNS query to find the IP address of the server that hosts maps.google.com. if found somewhere

Browser initiates a TCP connection with the server.

The browser sends an HTTP request to the web server.

The browser displays the HTML content (for HTML responses which is the most common).

The server handles the request and sends back a response.



 iterator in vanila javascript

object 
for in   (based on index)
for of  (based on value)

Array foreach




var ints = [ 1, 2, 3, 4, 5 ];

function indexOf(arr, test) {
  
  return BST(arr , 0 , arr.length, test)
}


function BST(arr , min , max , test){
  console.log('min , max',min,max);
  var mid = Math.floor((min + max)/2);
  if(min<max){
      if(test == arr[mid] ){
        return mid;
      }else if(test > arr[mid]){

      return BST(arr ,mid,max ,test);
    }else if(test  < arr[mid]){
      return BST(arr ,min,mid ,test);
    }
  }else{
    
    return -1;
    
  }  

}




///////////


align on div to center of another Div 


Solutions 1 :-

div.outer {
    display: table-cell;
    width: 500px;
    height: 500px;
    background: gray;
    vertical-align: middle;
    text-align: center;
}

div.inner {
    display: inline-block;
    width: 200px;
    height: 200px;
    background: red;
}

solution 2 :-
.cn {
  position: relative;
  width: 500px;
  height: 500px;
}

.inner {
  position: absolute;
  top: 50%; left: 50%;
  transform: translate(-50%,-50%);
  width: 200px;
  height: 200px;
}


Solution 3: -
div.outer {
   display: flex;
  justify-content: center;
    width: 500px;
    height: 500px;
    background: gray;
  
}

div.inner {
   background: gold;
  align-self: center;
  padding: 2rem;
}

The CSS transform property lets you modify the coordinate space of the CSS visual formatting model. Using it, elements can be translated, rotated, scaled, and skewed.
(common wald shift coordinates)




Difference between Inline vs inline-block vs block

Inline elements:

respect left & right margins and padding, but not top & bottom
cannot have a width and height set
allow other elements to sit to their left and right.
see very important side notes on this here.

Block elements:

respect all of those
force a line break after the block element

Inline-block elements:

allow other elements to sit to their left and right
respect top & bottom margins and padding
respect height and width




An inline element has no line break before or after it, and it tolerates HTML elements next to it.
A block element has some whitespace above and below it and does not tolerate any HTML elements next to it.
An inline-block element is placed as an inline element (on the same line as adjacent content), but it behaves as a block element.



Flex in css   

example
div{
   width: 220px;
    height: 300px;
    border: 1px solid black;
    display: -webkit-flex; /* Safari */
    display: flex;
    flex-wrap:wrap;
}


vertical-align  :-

The vertical-align CSS property specifies the vertical alignment of an inline or table-cell box.

Default font size:-
The default text size in browsers is 16px. So, the default size of 1em is 16px.



str.substring(indexStart, [indexEnd])

SubString 
If indexStart is greater than indexEnd, then the effect of substring() is as if the two arguments were swapped; for example, str.substring(1, 0) == str.substring(0, 1).



Event Deligation 

// Get the parent DIV, add click listener...
  document.getElementById("myDiv").addEventListener("click",function(e) {
// e.target was the clicked element
if(e.target && e.target.nodeName == "A") {
    // Get the CSS classes
    var classes = e.target.className.split(" ");
    // Search for the CSS class!
    if(classes) {
        // For every CSS class the element has...
        for(var x = 0; x < classes.length; x++) {
            // If it has the CSS class we want...
            if(classes[x] == "classA") {
                // Bingo!
                console.log("Anchor element clicked!");
                // Now do something here....
            }
        }
    }

  }
});




Bind 


this.x = 9;    // this refers to global "window" object here in the browser
var module = {
  x: 81,
  getX: function() { return this.x; }
};

module.getX(); // 81

var retrieveX = module.getX;
 retrieveX();   
 // returns 9 - The function gets invoked at the global scope

// Create a new function with 'this' bound to module
// New programmers might confuse the
// global var x with module's property x

var boundGetX = retrieveX.bind(module);

boundGetX(); // 81



Borrowing Functions with Apply and Call (A Must Know)



// Make a quick copy and save the results in a real array:​
                // First parameter sets the "this" value​
                var newArray = Array.prototype.slice.call (anArrayLikeObj, 0);


                 console.log (Array.prototype.pop.call (anArrayLikeObj));

While the syntax of this function is almost identical to that of apply(), the fundamental difference is that call() accepts an argument list, while apply() accepts a single array of arguments.



Block zooming for web page 

<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />



create 3 colum layout here 1st and last coloum width is fixed and middle on is flexible .
solution :- used table for container  and table-cell for colom .




does sum of w number in a array to match to a given number

findSum([6,1,4,5,7],3) false
findSum([6,1,2,5,7],3) true

solve it by doing a difference and putting it in obect





# JavaScript /DOM,HTML,CSS


***************Raference*****************

https://github.com/h5bp/Front-end-Developer-Interview-Questions

https://en.wikipedia.org/wiki/DOM_events


https://www.w3.org/TR/DOM-Level-2-Events/events.html

https://javascript.info/onload-ondomcontentloaded

****************************************


## Concurent connections with Browsers

IE7 allowed only two concurrent connections per host. But most browsers today allow more than that. 
IE8 allows 6 concurrent connections, Chrome allows 6, and Firefox allows 8.

So if your web page only has 6 images, for example, then it'd really be pointless to spread your images across multiple subdomains.


##DOM

"The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document."


The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

## Window vs Document 

window

Each browser tab has its own top-level window object

document

Each window object has a document object to be rendered. 


##Browser events
  Mouse events:
      click , contextmenu , mousehover etc
  Keybord Events:
      keyup , keydown ,KeyPress
  HTML frame/object
      load , unload ,scroll
  HTML form
      select , focus , submit , reset etc
  User interface
      focusin
  Mutation Event
      DOMSubtreeModified , DOMNodeInserted  etc
  Progress Events
      load , error ,abort etc




##Event flow


Consider the situation when there are 2 elements nested together. Both have event handlers registered on the same event type, say "click". When the user clicks on the inner element, there are two possible ways to handle it:

Trigger the elements from outer to inner (event capturing). This model is implemented in Netscape Navigator.
Trigger the elements from inner to outer (event bubbling). This model is implemented in Internet Explorer and other browsers.


W3C takes a middle position in this struggle. Events are first captured until it reaches the target element, and then bubbled up. During the event flow, an event can be responded to at any element in the path (an observer) in either phase by causing an action, and/or by stopping the event (with method event.stopPropagation() for W3C-conforming browsers and command event.cancelBubble = true for Internet Explorer), and/or by cancelling the default action for the event.


#Event object


The Event object provides a lot of information about a particular event, including information about target element, key pressed, mouse button pressed, mouse position, etc. Unfortunately, there are very serious browser incompatibilities in this area. Hence only the W3C Event object is discussed in this article.

Event properties :-


DOMString         type           The name of the event (case-insensitive in DOM level 2 but case-sensitive in DOM level 3 [15]).
EventTarget       target         Used to indicate the EventTarget to which the event was originally dispatched.
EventTarget       currentTarget  Used to indicate the EventTarget whose EventListeners are currently being processed.
unsigned short    eventPhase     Used to indicate which phase of event flow is currently being evaluated.
boolean           bubbles        Used to indicate whether or not an event is a bubbling event.
boolean           cancelable     Used to indicate whether or not an event can have its default action prevented.
DOMTimeStamp      timeStamp      Used to specify the time (in milliseconds relative to the epoch) at which the event was created.




##Event handling models

#DOM Level 0

This event handling model was introduced by Netscape Navigator, and remains the most cross-browser model as of 2005.[citation needed] There are two model types: inline model and traditional model.

*Inline model
In the inline model,[16] event handlers are added as attributes of elements. In the example below, an alert dialog box with the message "Hey Joe" appears after the hyperlink is clicked. The default click action is cancelled by returning false in the event handler.

    <a href="http://www.example.com" onclick="triggerAlert('Joe'); return false;">Joe</a>!</p>

    function triggerAlert(name) {
          window.alert("Hey " + name);
    }


*Traditional model
In the traditional model,event handlers can be added/removed by scripts. Like the inline model, each event can only have one event handler registered. The event is added by assigning the handler name to the event property of the element object. To remove an event handler, simply set the property to null:

    var triggerAlert = function () {
      window.alert("Hey Joe");
    };
    
    // Assign an event handler
    document.onclick = triggerAlert;
    
    // Assign another event handler
    window.onload = triggerAlert;
    
    // Remove the event handler that was just assigned
    window.onload = null;



#DOM Level 2


The W3C designed a more flexible event handling model in DOM Level 2


addEventListener       Allows the registration of event listeners on the event target.
Arguments 
  DOMString      type
  EventListener  listener
  boolean        useCapture
removeEventListener    Allows the removal of event listeners from the event target.  
 Arguments
  DOMString       type
  EventListener  listener
  boolean        useCapture
dispatchEvent    Allows sending the event to the subscribed event listeners.
 Arguments 
  Event evt


document.addEventListener( "click", heyJoe, true );  // capture phase

window.addEventListener( "load", heyJoe, false );  // bubbling phase



 Some useful things to know :

To prevent an event bubbling, developers must set the event's cancelBubble property.
To prevent the default action of the event to be called, developers must set the event's "returnValue" property.
The this keyword refers to the global window object.






## async and defer

 Attributes async and defer work only for external scripts. They are ignored if there’s no src.


Both of them tell the browser that it may go on working with the page, and load the script “in background”, then run the script when it loads. So the script doesn’t block DOM building and page rendering.

##async Vs defer (differ in Order , DOMContentLoaded )


 *Order
  Scripts with async execute in the load-first order. Their document order doesn’t matter – which loads first runs first.

  Scripts with defer always execute in the document order (as they go in the document).

*DOMContentLoaded

  Scripts with async may load and execute while the document has not yet been fully downloaded. That happens if scripts are small or cached, and the document is long enough.

  Scripts with defer execute after the document is loaded and parsed (they wait if needed), right before DOMContentLoaded.


#DOMContentLoaded Vs load

The DOMContentLoaded event is fired when the document has been completely loaded and parsed, without waiting for stylesheets, images, and subframes to finish loading .
the load event can be used to detect a fully-loaded page.

##readyState

The document.readyState property gives us information about it. There are 3 possible values:

"loading" – the document is loading.
"interactive" – the document was fully read.
"complete" – the document was fully read and all resources (like images) are loaded too.

function work() { /*...*/ }

if (document.readyState == 'loading') {
  document.addEventListener('DOMContentLoaded', work);
} else {
  work();
}

*readystatechange event that triggers when the state changes

document.addEventListener('readystatechange', () => console.log(document.readyState))







## Event Deligation 

Event delegation allows us to attach a single event listener, to a parent element, that will fire for all descendants matching a selector, whether those descendants exist now or are added in the future.

Event delegation refers to the process of using event propagation (bubbling) to handle events at a higher level in the DOM than the element on which the event originated. It allows us to attach a single event listener for elements that exist now or in the future.




##New Elements in HTML5

 #New Semantic/Structural Elements
 <article>  <details>

 #New Form Elements
 <datalist>
 #New Input Types
 email ,month ,number ,range ,search ,tel ,time ,url ,week

 #HTML5 - New Attribute Syntax


 #HTML5 Graphics

 #New Media Elements
 vedio ,audio 


 #HTML5 API
 HTML5 Geolocation ,HTML5 Drag and Drop ,HTML5 Local Storage , HTML5 Web Workers  , HTML5 Server-Sent Events



## CSS3
border-radius ,  box-shadow , text-shadow  , text-stroke ,Multiple Backgrounds , background-size , text-overflow , Flexible Box Model , Resize , Transition
 

*************************** JavaScript ***************************




##CallBack 

A callback function, also known as a higher-order function, is a function that is passed to another function (let’s call this other function “otherFunction”) as a parameter, and the callback function is called (or executed) inside the otherFunction. A callback function is essentially a pattern (an established solution to a common problem), and therefore, the use of a callback function is also known as a callback pattern.


var friends = ["Mike", "Stacy", "Andy", "Rick"];
​
friends.forEach(function (eachName, index){
console.log(index + 1 + ". " + eachName); // 1. Mike, 2. Stacy, 3. Andy, 4. Rick​
});


Callback Functions Are Closures

When we pass a callback function as an argument to another function, the callback is executed at some point inside the containing function’s body just as if the callback were defined in the containing function. This means the callback is a closure. Read my post, Understand JavaScript Closures With Ease for more on closures. As we know, closures have access to the containing function’s scope, so the callback function can access the containing functions’ variables, and even the variables from the global scope.



Implement Callback

function getInput(options, callback) {
    allUserData.push(options);
​
    // Make sure the callback is a function​
    if (typeof callback === "function") {
    // Call it, since we have confirmed it is callable​
        callback(options);
    }
}





#Clouser


A closure is an inner function that has access to the outer (enclosing) function’s variables—scope chain. The closure has three scope chains: it has access to its own scope (variables defined between its curly brackets), it has access to the outer function’s variables, and it has access to the global variables.


function showName (firstName, lastName) { 
​var nameIntro = "Your name is ";
    // this inner function has access to the outer function's variables, including the parameter​
​function makeFullName () {         
​return nameIntro + firstName + " " + lastName;     
}
​
​return makeFullName (); 
} 
​
showName ("Michael", "Jackson"); //


 #IIFE

 (function () {
    var foo = "bar";

    // Outputs: "bar"
    console.log(foo);
})();

(function(){ /* code */ }());


!function(){ /* code */ }();

~function(){ /* code */ }();

-function(){ /* code */ }();

+function(){ /* code */ }();



# Promise


Promises are not callbacks. A promise represents the future result of an asynchronous operation.

Understanding JavaScript Promises. A promise represents the eventual result of an asynchronous operation. It is a placeholder into which the successful result value or reason for failure will materialize.

The Promise constructor takes a function (an executor) that will be executed immediately and passes in two functions: resolve , which must be called when the Promise is resolved (passing a result), and reject , when it is rejected (passing an error).




var  P1 = new Promise(function(resolve, reject) {
  
  setTimeout(function(){
    resolve("Success!"); // Yay! Everything went well!
  }, 250);
});

P1.then(function(successMessage){
 //run when promise is resolved
});

var P2 = new Promise(function(resolve, reject) {

  if (true) {
    resolve("Stuff worked!");
  }
  else {
    reject(Error("It broke"));
  }
});

P2.then(function(successMessage){
  //run when promise is resolved
}).catch(function(err){
	 //run for error
});

Promise.all([P1, P2]).then(function() {
  // run all promise resolved
}, function() {
  // one or more failed
});


Promise.race([P1, P2]).then(function() {
  // run when any one resolved
}, function() {
  // one or more failed
});



##REST API
Representational state transfer (REST) or RESTful Web services are one way of providing interoperability between computer systems on the Internet


##REST vs SOAP (Simple Object Access Protocol) web services
http/s   others
can use any format     XML

## Canvas VS SVG

Canvas draws 2D graphics, on the fly (with a JavaScript). SVG is XML based, which means that every element is available within the SVG DOM. You can attach JavaScript event handlers for an element. In SVG, each drawn shape is remembered as an object.





## Web Socket 

The HTML5 WebSockets specification defines an API that enables web pages to use the WebSockets protocol for two-way communication with a remote host. It introduces the WebSocket interface and defines a full-duplex communication channel that operates through a single socket over the Web. HTML5 WebSockets provide an enormous reduction in unnecessary network traffic and latency compared to the unscalable polling and long-polling solutions that were used to simulate a full-duplex connection by maintaining two connections.







var exampleSocket = new WebSocket("ws://www.example.com/socketserver", "protocolOne");

var exampleSocket = new WebSocket("ws://www.example.com/socketserver", ["protocolOne", "protocolTwo"]);
Once the connection is established (that is, readyState is OPEN), exampleSocket.protocol will tell you which protocol the server selected.


 var msg = {
    type: "message",
    text: document.getElementById("text").value,
    id:   clientID,
    date: Date.now()
  };

  // Send the msg object as a JSON-formatted string.
  exampleSocket.send(JSON.stringify(msg));


exampleSocket.onopen = function (event) {
  exampleSocket.send("Here's some text that the server is urgently awaiting!"); 
};


 



exampleSocket.onmessage = function (event) {
  console.log(event.data);
    var msg = JSON.parse(event.data);
}



## web Worker


A web worker is a JavaScript running in the background, without affecting the performance of the page.



if(typeof(Worker) !== "undefined") {
        if(typeof(w) == "undefined") {
            w = new Worker("demo_workers.js");
        }
        w.onmessage = function(event) {
            document.getElementById("result").innerHTML = event.data;
        };
    } else {
        document.getElementById("result").innerHTML = "Sorry! No Web Worker support.";
    }



## Server-Sent Events  One Way Messaging
Server-Sent Events allow a web page to get updates from a server.


Events	Description
onopen	When a connection to the server is opened
onmessage	When a message is received
onerror	When an error occurs


var source = new EventSource("demo_sse.php");
source.onmessage = function(event) {
    document.getElementById("result").innerHTML += event.data + "<br>";
};




## create object 


var a = new Object();  //constructor 


var obj = {};
Object.defineProperty(obj, 'key', {
  __proto__: null, // no inherited properties
  value: 'static'  // not enumerable
                   // not configurable
                   // not writable
                   // as defaults
});

// being explicit
Object.defineProperty(obj, 'key', {
  enumerable: false,
  configurable: false,
  writable: false,
  value: 'static'
});



## Inharitance  


function Shape() {
  this.x = 0;
  this.y = 0;
}

// superclass method
Shape.prototype.move = function(x, y) {
  this.x += x;
  this.y += y;
  console.info('Shape moved.');
};

// Rectangle - subclass
function Rectangle() {
  Shape.call(this); // call super constructor.
}

// subclass extends superclass
Rectangle.prototype = Object.create(Shape.prototype);
Rectangle.prototype.constructor = Rectangle;

var rect = new Rectangle();

rect.move(1, 1); // Outputs, 'Shape moved.'


## Design patterns 

https://code.tutsplus.com/tutorials/understanding-design-patterns-in-javascript--net-25930




#Creational patterns
 focus on ways to create objects or classes. This may sound simple (and it is in some cases), but large applications need to control the object creation process.




 Module Design Pattern

JavaScript modules are the most prevalently used design patterns for keeping particular pieces of code independent of other components. This provides loose coupling to support well-structured code.

For those that are familiar with object-oriented languages, modules are JavaScript "classes". One of the many advantages of classes is encapsulation - protecting states and behaviors from being accessed from other classes. The module pattern allows for public and private (plus the lesser-know protected and privileged) access levels.


Modules should be Immediately-Invoked-Function-Expressions (IIFE) to allow for private scopes - that is, a closure that protect variables and methods (however, it will return an object instead of a function). This is what it looks like:

var HTMLChanger = (function() {
  var contents = 'contents'

  var changeHTML = function() {
    var element = document.getElementById('attribute-to-change');
    element.innerHTML = contents;
  }

  return {
    callChangeHTML: function() {
      changeHTML();
      console.log(contents);
    }
  };

})();


Revealing Module Pattern

A variation of the module pattern is called the Revealing Module Pattern. The purpose is to maintain encapsulation and reveal certain variables and methods returned in an object literal. 

var Exposer = (function() {
  var privateVariable = 10;

  var privateMethod = function() {
    console.log('Inside a private method!');
    privateVariable++;
  }

  var methodToExpose = function() {
    console.log('This is a method I want to expose!');
  }

  var otherMethodIWantToExpose = function() {
    privateMethod();
  }

  return {
      first: methodToExpose,
      second: otherMethodIWantToExpose
  };
})();

Exposer.first();        // Output: This is a method I want to expose!
Exposer.second();       // Output: Inside a private method!
Exposer.methodToExpose; // undefined



Prototype Design Pattern

The Prototype design pattern relies on the JavaScript prototypical inheritance. The prototype model is used mainly for creating objects in performance-intensive situations.

var TeslaModelS = function() {
  this.numWheels    = 4;
  this.manufacturer = 'Tesla';
  this.make         = 'Model S';
}

TeslaModelS.prototype.go = function() {
  // Rotate wheels
}

TeslaModelS.prototype.stop = function() {
  // Apply brake pads
}


Revealing Prototype Pattern

The Revealing Prototype Pattern provides encapsulation with public and private members since it returns an object literal.


var TeslaModelS = function() {
  this.numWheels    = 4;
  this.manufacturer = 'Tesla';
  this.make         = 'Model S';
}

TeslaModelS.prototype = function() {

  var go = function() {
    // Rotate wheels
  };

  var stop = function() {
    // Apply brake pads
  };

  return {
    pressBrakePedal: stop,
    pressGasPedal: go
  }

}();



Singleton

A Singleton is an object which can only be instantiated one time. Repeated calls to its constructor return the same instance and in this way one can ensure that they don't accidentally create, say, two Users in a single User application



var printer = (function () {

  var printerInstance;

  function create () {

    function print() {
     
    }

    function turnOn() {
         }

    return {
       print: print,
      turnOn: turnOn
    };
  }

  return {
    getInstance: function() {
      if(!printerInstance) {
        printerInstance = create();
      }
      return printerInstance;
    }
  };

 
})();

Factory 
 
will hide  actual object creation process , provide common interface that can take parameter and decide what kind of object need to be created 


#Structural design 
patterns focus on ways to manage relationships between objects so that your application is architected in a scalable way. A key aspect of structural patterns is to ensure that a change in one part of your application does not affect all other parts.



focus on communication between objects.


Composite Pattern
The composite pattern is another pattern that you probably have used before without any realization.

The composite pattern says that a group of objects can be treated in the same manner as an individual object of the group.

$('.myList').addClass('selected');
$('#myItem').addClass('selected');
 
//dont do this on large tables, it's just an example.
$("#dataTable tbody tr").on("click", function(event){
    alert($(this).text());
});
 
$('#myButton').on("click", function(event) {
    alert("Clicked.");
});


Facade Pattern
Here's another common pattern that we take for granted. In fact, this one is one of my favorites because it's simple, and I've seen it being used all over the place to help with browser inconsistencies. Here's what the Facade pattern is about:

The Facade Pattern provides the user with a simple interface, while hiding it's underlying complexity.

$(document).ready(function() {
 
    //all your code goes here...
 
});


#Behavioral patterns 

Observer Design Pattern

In the Observer Pattern, a subject can have a list of observers that are interested in it's lifecycle. Anytime the subject does something interesting, it sends a notification to its observers. If an observer is no longer interested in listening to the subject, the subject can remove it from its list.






##isNAN

isNaN(true);      // false
isNaN(null);      // false
isNaN(37);        // false

Number.isNaN = Number.isNaN || function(value) {     
    return value !== value;
}

NAN===NAN is false



## AngularJS 


AngularJS Life Cycle
The three phases of the life cycle of an AngularJS application happen each time a web page is loaded in the browser. The following sections describe these phases of an AngularJS application.

The Bootstrap Phase
The first phase of the AngularJS life cycle is the bootstrap phase, which occurs when the AngularJS JavaScript library is downloaded to the browser. AngularJS initializes its own necessary components and then initializes your module, which the ng-app directive points to. The module is loaded, and any dependencies are injected into your module and made available to code within the module.

The Compilation Phase
The second phase of the AngularJS life cycle is the HTML compilation stage. Initially when a web page is loaded, a static form of the DOM is loaded in the browser. During the compilation phase, the static DOM is replaced with a dynamic DOM that represents the AngularJS view.

This phase involves two parts: traversing the static DOM and collecting all the directives and then linking the directives to the appropriate JavaScript functionality in the AngularJS built-in library or custom directive code. The directives are combined with a scope to produce the dynamic or live view.

The Runtime Data Binding Phase
The final phase of the AngularJS application is the runtime phase, which exists until the user reloads or navigates away from a web page. At that point, any changes in the scope are reflected in the view, and any changes in the view are directly updated in the scope, making the scope the single source of data for the view.

AngularJS behaves differently from traditional methods of binding data. Traditional methods combine a template with data received from the engine and then manipulate the DOM each time the data changes. AngularJS compiles the DOM only once and then links the compiled template as necessary, making it much more efficient than traditional methods.





# CSS

position 


There are four different position values:

static
relative
fixed
absolute


static :-
HTML elements are positioned static by default.

Static positioned elements are not affected by the top, bottom, left, and right properties.

position: relative;
An element with position: relative; is positioned relative to its normal position.

Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.


position: fixed;
An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.

An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).


position: absolute;
An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

z-index ((position:absolute, position:relative, or position:fixed))
The z-index property specifies the stack order of an element. An element with greater stack order is always in front of an element with a lower stack order. Note: z-index only works on positioned elements . Default value: auto.


Note: If two positioned elements overlap without a z-index specified, the element positioned last in the HTML code will be shown on top.



# Box model (box-sizing)


All HTML elements can be considered as boxes. In CSS, the term "box model" is used when talking about design and layout.
The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. 



Important: When you set the width and height properties of an element with CSS, you just set the width and height of the content area. To calculate the full size of an element, you must also add padding, borders and margins.


box-sizing: border-box;

content-box
This is the initial and default value as specified by the CSS standard. The width and height properties are measured including only the content, but not the padding, border or margin


border-box
The width and height properties include the content, the padding and border, but not the margin









What are Pseudo-classes?
A pseudo-class is used to define a special state of an element.

For example, it can be used to:

Style an element when a user mouses over it
Style visited and unvisited links differently
Style an element when it gets focus

a:link {
    color: #FF0000;
}

/* visited link */
a:visited {
    color: #00FF00;
}




What are Pseudo-Elements?
A CSS pseudo-element is used to style specified parts of an element.

For example, it can be used to:

Style the first letter, or line, of an element
Insert content before, or after, the content of an element

selector::pseudo-element {
    property:value;
}


p::first-line {
    color: #ff0000;
    font-variant: small-caps;
}


CSS Combinators

A combinator is something that explains the relationship between the selectors.

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS3:

descendant selector (space)
child selector (>)
adjacent sibling selector (+)
general sibling selector (~)




# JQuery
The jQuery library contains the following features:

HTML/DOM manipulation
CSS manipulation
HTML event methods
Effects and animations
AJAX
Utilities




###Roman No converter 



function converToRoman(input){
  console.log(input);
  
  var riman= ["M","XM","CM","D","CD","C","XC","L","XL","X","IX","V","IV","I"];
    var numeric= [1000, 990, 900, 500,400, 100, 90, 50, 40, 10, 9, 5, 4, 1];
  var i=0;
  var output ="";
  while(input && i<numeric.length){
    if(input-numeric[i] >=0){
      output+=riman[i]
      input -= numeric[i];
    }else{
      i++;
    }
    
  }
   
   console.log(output);
 
 
}


function romanize(num) {
  var lookup = {M:1000,CM:900,D:500,CD:400,C:100,XC:90,L:50,XL:40,X:10,IX:9,V:5,IV:4,I:1},roman = '',i;
  for ( i in lookup ) {
    while ( num >= lookup[i] ) {
      roman += i;
      num -= lookup[i];
    }
  }
  return roman;
}


## Fabi

function Fab(5){
  
  if(n==0 || n==1)  
   return 1;
   else
   return Fab(n-2)+Fab(n-1);

}




## tree looping 


Loop arround to create trees

*
**
***
****


function myTree(n){
  for (var i=0;i<n;i++){
       var str="";
    for (var j=0;j<=i;j++){
      str+="*";
    }
    console.log(str);
  }
}



      *
     **
    ***
   ****
  *****

function reverTree(n){
 for(var i=n;i >0;i--){
  var str="";
  for (var j=1;j<=n;j++){
    if(i>j){
    str+=" ";
    }else{
    str+="*";
    }
  } console.log(str);
 }

}


## check its number or not without using build in functions 

function isInteger (x) {
    return (x^0===x);
}


## Sum 2 large number without using + operation 


## delete odd number from linked list 




## LRU cache Implentations

should have 

get(key)       - return value or -1;
put(key,value) - return size


var LRUCache = function (maxsize) {
  this._keys = [];
  this._items = {};
  this._expires = {};
  this._size = 0;
  this._maxsize = maxsize || 1024;
}

LRUCache.prototype = {

  set: function (key, value, callback) {

   var keys = this._keys;
   var items = this._items;
   var expires = this._expires;
   var size = this._size ;
   var maxsize = this._maxsize;


   if(size >=maxsize){
		// create space 

		// get key of last recently used 

		keys.sort(function(a,b){
		  if (expires[a] > expires[b]) return -1;
          if (expires[a] < expires[b]) return 1;
          else return 0;
		});
	  size--;
      delete expires[keys[size]];
      delete items[keys[size]];
   }

   keys[size] = key;
   items[key] = value;
   expires[key] = Date.now();
   size++;

   this._keys = keys;
   this._items = items;
   this._expires = expires;
   this._size = size;

    if (callback) return callback(size);



  }

  get: function(key,callback){

   var item = this._items[key];
   if(item){
     this._expires[key] = Date.now();
   }
   if (callback) return callback(item);
    return item;

  }

  }




/* Angular JS */

How to make state or route case insensitive 
 $routeProvider.
        when('/', { controller: 'TmpCtrl', templateUrl: '/app/home.html' }).
        when('/foo', { controller: 'TmpCtrl', templateUrl: '/app/foo.html', caseInsensitiveMatch: true }).  
        otherwise({ redirectTo: '/' });


  app.config(function ($urlRouterProvider) {
  // Here's an example of how you might allow case insensitive urls
   $urlRouterProvider.rule(function ($injector, $location) {
   //what this function returns will be set as the $location.url
    var path = $location.path(), normalized = path.toLowerCase();
    if (path != normalized) {
        //instead of returning a new url string, I'll just change the $location.path directly so I don't have to worry about constructing a new url string and so a new state change is not triggered
        $location.replace().path(normalized);
    }
    // because we've returned nothing, no state change occurs
});}



default router 
 $urlRouterProvider.otherwise('/default')
how to remove # from router 
$locationProvider.html5Mode(true);





AngularJS Life Cycle
The three phases of the life cycle of an AngularJS application happen each time a web page is loaded in the browser. The following sections describe these phases of an AngularJS application.

The Bootstrap Phase
The first phase of the AngularJS life cycle is the bootstrap phase, which occurs when the AngularJS JavaScript library is downloaded to the browser. AngularJS initializes its own necessary components and then initializes your module, which the ng-app directive points to. The module is loaded, and any dependencies are injected into your module and made available to code within the module.

The Compilation Phase
The second phase of the AngularJS life cycle is the HTML compilation stage. Initially when a web page is loaded, a static form of the DOM is loaded in the browser. During the compilation phase, the static DOM is replaced with a dynamic DOM that represents the AngularJS view.

This phase involves two parts: traversing the static DOM and collecting all the directives and then linking the directives to the appropriate JavaScript functionality in the AngularJS built-in library or custom directive code. The directives are combined with a scope to produce the dynamic or live view.

The Runtime Data Binding Phase
The final phase of the AngularJS application is the runtime phase, which exists until the user reloads or navigates away from a web page. At that point, any changes in the scope are reflected in the view, and any changes in the view are directly updated in the scope, making the scope the single source of data for the view.

AngularJS behaves differently from traditional methods of binding data. Traditional methods combine a template with data received from the engine and then manipulate the DOM each time the data changes. AngularJS compiles the DOM only once and then links the compiled template as necessary, making it much more efficient than traditional methods.



#################################
Strict mode 

'use strict';

ECMAScript 5's strict mode is a way to opt in to a restricted variant of JavaScript

Strict mode makes several changes to normal JavaScript semantics. 
First, strict mode eliminates some JavaScript silent errors by changing them to throw errors.
Second, strict mode fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that's not strict mode. 

Third, strict mode prohibits some syntax likely to be defined in future versions of ECMAScript.


example 1:-

'use strict';
var v = "Hi! I'm a strict mode script!";

example 2:-
function strict() {
  // Function-level strict mode syntax
  'use strict';
  function nested() { return 'And so am I!'; }
  return "Hi!  I'm a strict mode function!  " + nested();
}



Changes in strict mode

Strict mode changes both syntax and runtime behavior.
Changes generally fall into these categories: changes converting mistakes into errors (as syntax errors or at runtime), 
 changes simplifying how the particular variable for a given use of a name is computed, changes simplifying eval and arguments, 
 changes making it easier to write "secure" JavaScript, and changes anticipating future ECMAScript evolution.


* Converting mistakes into errors


First, strict mode makes it impossible to accidentally create global variables.

'use strict';
                       // Assuming a global variable mistypedVariable exists
mistypeVariable = 17; // this line throws a ReferenceError due to the 
                       // misspelling of variable




Second, strict mode makes assignments which would otherwise silently fail to throw an exception.

'use strict';


// Assignment to a non-writable global
var undefined = 5; // throws a TypeError
var Infinity = 5; // throws a TypeError

// Assignment to a non-writable property
var obj1 = {};
Object.defineProperty(obj1, 'x', { value: 42, writable: false });
obj1.x = 9; // throws a TypeError

// Assignment to a getter-only property
var obj2 = { get x() { return 17; } };
obj2.x = 5; // throws a TypeError

// Assignment to a new property on a non-extensible object
var fixed = {};
Object.preventExtensions(fixed);
fixed.newProp = 'ohai'; // throws a TypeError


Third, strict mode makes attempts to delete undeletable properties throw 

'use strict';
delete Object.prototype; // throws a TypeError


Fourth, strict mode prior to Gecko 34 requires that all properties named in an object literal be unique.
'use strict';
var o = { p: 1, p: 2 }; // !!! syntax error


Fifth, strict mode requires that function parameter names be unique. In normal code the last duplicated argument hides previous identically-named arguments.

function sum(a, a, c) { // !!! syntax error
  'use strict';
  return a + b + c; // wrong if this code ran
}

Sixth, strict mode in ECMAScript 5 forbids octal syntax.
'use strict';
var sum = 015 + // !!! syntax error
          197 +
          142;


* Simplifying variable uses

First, strict mode prohibits with. 

Second, eval of strict mode code does not introduce new variables into the surrounding scope. In normal code eval("var x;") introduces a variable x into the surrounding function or the global scope. This means that, in general, in a function containing a call to eval every name not referring to an argument or local variable must be mapped to a particular definition at runtime 

* Making eval and arguments simpler

All these attempts to do so are syntax errors:

'use strict';
eval = 17;
arguments++;
++eval;


arguments.callee is no longer supported. 

"Securing" JavaScript


########################



https://developers.google.com/web/fundamentals/performance/critical-rendering-path/page-speed-rules-and-recommendations



//////// 
 Sum all number inside a object 

 var obj ={ a:10 ,b:20 , c :[ 10,20,30, { a:10}]}

function SumObj(obj){
 var sum=0;
  for (var val of obj){

     if(typeof val =='number'){
       sum +=val
     }else{
      sum +=SumObj(val);
     }
  }
  return sum;
 }


 Balance paranthesis 

 currying implementation to write a function  intiCount ??
   let incr = intiCount(5);
   incr() // 6
   incr() // 7




// Implementation of context swtiching 
var a = {
  name:'Vivek',
  prop: {
    name:'Aravind',
    getName: function(test) {
      console.log(this.name+' '+test);
    }
  }
}
a.prop.getName();
a.prop.getName.apply(a,['venkatachari']);
a.prop.getName.call(a,'venkatachari');
b = a.prop.getName.bind(a);
b('Venkatachari');



// reverse array or string in optimized way


custom directive


E for Element name
A for Attribute
C for Class
M for Comment
By default the value is EA, meaning that both Element names and attribute names can invoke the directive.


<div my-isolated-scope-with-model-and-function 
     datasource="customer" 
     action="changeData()">
</div>


angular.module('directivesModule').directive('myIsolatedScopeWithModelAndFunction', function () {
    return {
    restrict : "A",
        scope: {
            datasource: '=',
            action: '&'
        },
        template: '<ul><li ng-repeat="prop in datasource">{{ prop }}</li></ul> ' +
                  '<button ng-click="action()">Change Data</button>'
    };
});




# SCSS

Browser concepts
whats is clouser 
why it is useful


At first glance, a closure is simply a function defined within another function. However, the power of closures is derived from the fact that the inner function remembers the environment in which it was created. In other words, the inner function has access to the outer function’s variables and parameters.




what is event deligation
bubbling

what is box model
Position 



DS 
Hash 


All anagrams 
n queen , break dollar








https://github.com/h5bp/Front-end-Developer-Interview-Questions 

interviewcake.com/






SASS /SCSS  Benefits

1. VARIABLES
2. @IMPORT    : - maintainanbility 
 Sass is a preprocessor (emphasis on the pre) that will pull in that file before it compiles the CSS.
The result is one CSS page that is handled by one HTTP request. What this means is that you can break up your css into smaller, more maintainable chunks while still only serving one page to the browser. Need to fix the text on the button? No more skimming style sheets looking for the pertinent button styles. Just open up your button partial and make the changes.  

What’s a partial? Just what they sound like. They are partial Sass files that contain little snippets of CSS that you can include in other Sass files. They are named by using a leading underscore followed by a name. _myFile.scss. The underscore lets Sass know that the file is only a partial file and that it should not be compiled into CSS. To import this partial you just have to add the @import to your file like so


3. COLOR FUNCTIONS

lighten($color, $amount) darken($color, $amount) rgba($color, $alpha)

4. MIXINS :-

Mixins make groups of CSS declarations that we can reuse throughout our site. CSS3 styles that require vendor prefixes are a perfect example of when to use a mixin. Instead of typing the same property over and over we write a mixin once then call that mixin anytime we want to use it. To declare a mixin we use the @mixin keyword.

To use our mixin we just use the @include keyword.

@mixin box-sizing($boxSize) {
  -webkit-box-sizing: $boxSize; 
     -moz-box-sizing: $boxSize; 
          box-sizing: $boxSize;
}

//use mixin
.mySelector {
    @include box-sizing(border-box);
}

5. @EXTEND

@extend is one of the most useful features that allows us to share a set of CSS properties from one selector to another.
Think of a pair of buttons, like an accept and decline button on a modal window. Since they are both buttons they’ll probably share most of the same styling but the decline button will have a red background to make it stand out. With Sass we write the default styles for all buttons then “extend” these styles to the decline button where we would add the red background.

.button {
 background: rgba($color, .8);
 color: lighten($color, 65%);
 border: 1px solid darken($color, 5%);
 padding: 1em;
 display: block;
 max-width: 200px;
}
.button-decline {
 @extend .button;
 background: red;
}











