# showcase-slider
A showcase slider displays the "best of" your content to users with a powerful, responsive slider. In Part II of our FlexSlider Series, [Solodev](https://www.solodev.com/) provides you with the code you need to add a showcase slider to your homepage using the fully responsive jQuery toolkit [FlexSlider by woothemes](https://woocommerce.com/flexslider/).

## Tutorial

For detailed instructions, view Solodev's [Building a Showcase Slider for your Website](https://www.solodev.com/blog/web-design/building-a-showcase-slider-for-your-website.stml) article.

## Demo

Check out a working example on [JSFiddle](https://jsfiddle.net/solodev/fxqLqs4a/).

## HTML

The flexslider has the following HTML markup.
```
<div class="outerWideSlider">
   <div class="wideSlider">
      <div class="flexslider" data-startat="0">
         <ul class="slides">
            <li>
               <img alt="" src="images/slide1.jpg">
               <div class="text-caption">
                  <div class="inner">
                     <h2>Slide #1</h2>
                     <p>This is the text for slide #1</p>
                  </div>
               </div>
            </li>
            <li>
               <img alt="" src="images/slide2.jpg">
               <div class="text-caption">
                  <div class="inner">
                     <h2>Slide #2</h2>
                     <p>This is the text for slide #1</p>
                  </div>
               </div>
            </li>
            <li>
               <img alt="" src="images/slide3.jpg">
               <div class="text-caption">
                  <div class="inner">
                     <h2>Slide #3</h2>
                     <p>This is the text for slide #1</p>
                  </div>
               </div>
            </li>
         </ul>
      </div>
   </div>
</div>
```
## JavaScript

The following JavaScript needs to be initiated on page load.

```
$(document).ready(function () {
$(".wideSlider").each(function () {
    var $this = $(this);
    var $slider = $this.find(".flexslider");
    var startat = $slider.attr("data-startat");
    if (startat = 0) {
    }
    $slider.flexslider({
      animation: 'slide',
      easing: 'linear', 
      slideshow: true, 
      slideshowSpeed: 7000, 
      animationLoop: true, 
      startAt: startat,
      controlNav: false,
      directionNav: true,
      nextText: " ",
      prevText: " ",
    });
  });
})
```

## CSS

All necessary CSS is in showcase-slider.css

## External Includes

This tutorial includes the following third party resources:

```
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/flexslider/2.6.2/flexslider.css">
<link rel="stylesheet" href="showcase-slider.css">

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-backstretch/2.0.4/jquery.backstretch.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/flexslider/2.6.2/jquery.flexslider.js"></script>
```
