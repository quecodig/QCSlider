<h1>QCSlider</h1>

It is a plugin which contains compatible code for viewing images, youtube videos and html5 videos
<strong>Use</strong>
* Include the jquery library
https://code.jquery.com/jquery.js

* Include JavaScript and CSS of QCSlider
```css/qc.slider.css?v1.2``` and ```qcslider.jquery.js?v1.4.2```
* HTML necessary for the operation
```html
<section class="slide">
	<div class="slider-container">
		<ul class="slider-wrapper" id="slider">
			<li class="slide-current"><!--Code for an image-->
				<img src="https://www.quecodigo.com/img/og_image.png" /><!--Code for an image-->
				<div class="capa"> </div><!--Custom HTML-->
			</li>
			<li class="video" data-type="video" data-video="https://www.quecodigo.com/video/ejemplo.mp4" data-muted="true"></li><!--HTML for HTML5 video with muted-->
			<li class="video" data-type="video" data-video="https://www.quecodigo.com/video/plugin_qcslider.mp4" data-muted="false"></li><!--HTML for HTML5 video-->
			<li class="video" data-type="youtube"data-video="sciFPlDs9XI" data-muted="true"></li><!--Code for youtube video-->
		</ul>
		<div class="drt-control control-left" id="lft-control"><</div>
          	<div class="drt-control control-right" id="rht-control">></div>
		<ul class="slider-controls" id="slider-controls"></ul>
		<div class="tempo-bar" id="barra"></div>
	</div>
</section>
```
* Initialize the slider, with the unique id
```js
$(document).ready(function($){
	$("#slider").QCslider({duration: 7000});
});
```
Demo: https://quecodig.github.io/QCSlider/
