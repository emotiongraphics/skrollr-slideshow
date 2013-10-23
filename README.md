
skrollr-slideshow 0.1.0
=====

skrollr plugin to make easy slide shows.

Documentation
=====

skrollr-slideshow is a simple slide show that uses skrollr, so objects fade in and fade out as you scroll down.

Each slide is an element one level below the element you supply.
An optional argument is how many pixels each element show stay on for. The default is 500.

```js
skrollr.slideShow.init(skrollrInstance, HTMLelement, numberOfPixelsPerSlide);
```

Example
=====
Super easy example. Put some stuff in a div. :

```html
<div class="skrllrSlideShow">

	<img src="img/photo.jpg">

	<img src="img/photo.jpg">
	
	<img src="img/photo.jpg">
	
	<div>Some text and a image.<img src="img/photo.jpg>"></div>
	
	<div>
		Child Elements will all be on the same slide.
		<ul>
			<li>This is all on one slide.</li>
			<li>This is still on the same slide</li>
		</ul>
	</div>
	
	<div>Next slide.</div>

	This will not be a slide, text needs to be in an element.

	<p>This is the last slide.</p>

</div>	
```
-Include skrollr and skrollr-slideshow.
-Init skrollr
-Init skrollr.slideshow, passing the instance of skrollr and the HTML element with your slides in it.

```js
<script type="text/javascript" src="js/skrollr.min.js"></script>
<script type="text/javascript" src="js/src/skrollr-show.js"></script>
<script type="text/javascript">
	var s = skrollr.init();
	skrollr.slideShow.init(s, "div.skrllrSlideShow");
</script>
```



Contributors
=====

* [Daniel McNeil](https://github.com/emotiongraphics)
