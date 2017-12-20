# dvlwjLoading

modified version of wdtLoading (https://github.com/needim/wdtLoading) to fit my taste.

# How to use

its very simple, just need to add this code to nested `<script></script>` before `</body>` tag.

```
	wdtLoading.start({
		category: 'default',
		speed: 1000
	});
	setTimeout(function(){
		wdtLoading.done();
	},1200);
```
