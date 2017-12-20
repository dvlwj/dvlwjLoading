# dvlwjLoading

modified version of wdtLoading (https://github.com/needim/wdtLoading) to fit my taste.

# Make a HTML smilliar to this

```
<div class="wdt-loading-screen">
	<div class="wdt-loading-phrases">
		<div class="wdt-loading-phrase-category" data-category="default">
			<div class="wdt-loading-phrase">text 1</div>
			<div class="wdt-loading-phrase">text 2</div>
			<div class="wdt-loading-phrase">text 3</div>
			<div class="wdt-loading-phrase">text 4</div>
			<div class="wdt-loading-phrase">text 5</div>
			<div class="wdt-loading-phrase">add as many as you want</div>
		</div>
	</div>
</div>
```

# Include CSS.

Put it to your head tag, its should be something like this:
```
<head>
	<link rel="stylesheet" href="css/wdtLoading.css">
</head>
```

# Include JavaScript

Put it to your body tag, just after your jQuery and before `</body>` tag, its should be something like this:
```
<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript" src="js/wdtLoading.js"></script>
</body>
```

# How to animate it ?

its very simple, just need to add this code to nested `<script></script>` after your wdtLoading.js and before `</body>` tag.
Its should be something like this:

```
<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript" src="js/wdtLoading.js"></script>
<script>
//to start the script use :
wdtLoading.start({
	category: 'default', //default stand for data-category="default" in HTML.
	speed: 1000
});
//to end the script use :
setTimeout(function(){
	wdtLoading.done();
},1200);
</script>
```

Remember to adjust the duration of animation (`wdtLoading.start`) with the Timeout duration (`setTimeout`).
