# jquery-equalbox
Simple jQuery plugin for equal height in html elements.  

#Installation
Install after the jQuery library
```javascript
<script src="path/to/jquery.equalbox.min.jss"></script>
```
#Important
You must be use the method: ```javascript $(window).load();``` for example:
```javascript
$(window).load(function(){
  $('body').equalbox();
});
```

#Listening the parent
The childs of parent element can listen and calculate the height, form example:
```html
<div data-equalbox>
	<div data-equalwatch></div>
	<div data-equalwatch></div>
</div>
```

#Listening other elements without be children directly
```html
<div data-equalbox="test" style="height: 100px"></div>
<div>
	<div data-equalwatch="test" id="foo"></div>
</div>
```
The element with id "foo" will have the hight with 100px.
