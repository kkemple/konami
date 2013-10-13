# KonamiJS
By Kurtis Kemple. Last Updated 10/12/2013

## About
Using this object, you can easily add an Easter Egg to your site/application for the page or an element ont the page.

## Options

 - code : an array of keycodes you want the user to enter / default is Konami code
 - cheat : the function you want to run whent the proper code is entered
 - elem : the element you want to bind the Easter Egg to / default is window object

## Instructions

First you must include the script file in the header of the page:

```javascript
<script src="js/vanilla.konami.js"></script>
```

Then at the bottom of the page you need to instantiate a new Konami object and pass in the configuration for the instance.

```javascript
var config = {
	cheat : function () {
		alert( "Konami!!" );
	}
}

var konami = new KONAMI( config );
```

And really that's it! This will alert "Konami!!" every time the Konami code is entered on the page. To narrow the scope of the event, simply invoke the instance on a different element like a div or input field.

