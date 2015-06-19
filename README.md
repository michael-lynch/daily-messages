#Daily Messages

Inspired by [Basecamp](https://basecamp.com/), Daily Messages is a simple, lightweight jQuery plugin used to display a custom message for each day of the week.

<a href="http://michael-lynch.github.io/daily-messages/" target="_blank">See a demo</a>

##Instructions

Include jQuery and the plugin in the head or footer of your page.

```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
<script src="/js/plugins/dailyMessages.min.js"></script>
```
    
Initialize the plugin targeting the class, ID or element that you want to display the message of the day. 

```js
$('.daily-message').dailyMessages({
	monday: "Case of the Mondays?",
	tuesday: "I know it's only Tuesday, but you can do it! ",
	wednesday: "Hump day baby!",
	thursday: "We all know Thursday is the new Friday.",
	friday: "Thank God! We made it. Happy Friday folks!",
	saturday: "It's Saturday fool! Stop using the Internets and go outside!",
	sunday: "NFL Sunday! Or maybe some Netflix? Chill.",
	success: function() {
		console.log('It worked!');
	},
	error: function(message) {
		console.log(message);
		$(this).remove();
	}
});
```
	
####Options

<ol>

<li>
monday: ""
<br />A string that defines the message that will be displayed on Mondays (default: `null`).
</li>

<li>
tuesday: ""
<br />A string that defines the message that will be displayed on Tuesdays (default: `null`).
</li>

<li>
wednesday: ""
<br />A string that defines the message that will be displayed on Wednesdays (default: `null`).
</li>

<li>
thursday: ""
<br />A string that defines the message that will be displayed on Thursdays (default: `null`).
</li>

<li>
friday: ""
<br />A string that defines the message that will be displayed on Fridays (default: `null`).
</li>

<li>
saturday: ""
<br />A string that defines the message that will be displayed on Saturdays (default: `null`).
</li>

<li>
sunday: ""
<br />A string that defines the message that will be displayed on Sundays (default: `null`).
</li>

<li>success: function()
<br />A callback function that runs if Daily Messages is successfull (default: `function()`). 
</li>

<li>error: function()
<br />A callback function that runs if Daily Messages fails (default: `function()`). 
</li>

</ol>		