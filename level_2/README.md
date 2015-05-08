### Level 2 - Clear Carving

#### Clearfix
Sometimes clearing is necessary. Floated items can be taller than non-floated content or even All children are floating. For all this cases we can apply 3 ways of clearing. They are:

1. Clear with a subsequent element: Requires sequence to stay intact - breaks if things move; Background / border do not extend. 
```html
<div>
  <img src="ski.jpg" alt="Skiing!" />
  <p>To successfully ski, simply do not fall.</p>
</div> 
<div class="intro">
  <p>Whee!</p>
</div>
```
```css
img {
  float: left;
}
.intro {
  clear: both;
}
```

2. Manual clearing: Requires an empty element; Might not be necessary later. 
```html
<div>
  <img src="ski.jpg" alt="Skiing!" />
  <p>To successfully ski, simply do not fall.</p>
  <div class="clear"></div>
</div>
```
```css
.clear {
  clear: both;
}
```
3. The clearfix.

```html    
<div class="group">
  <img src="ski.jpg" alt="Skiing!" />
  <p>To successfully ski, simply do not fall.</p>
</div>
```
```css
.group:before, .group:after {
  content: "";
  display: table;
}
.group :after {
  clear: both;
}
.group {
  zoom: 1; /* IE6&7 */
}
```
