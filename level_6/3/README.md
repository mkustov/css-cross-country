#### Image Crop
Sometimes we need to present images among our content. Probably they will be idealized by our designs as in different sizes that they were shot. On those cases the recommended is to *never* apply resizing directly to the `inline img` once it could deform the images during the resize. Check below the right and wrong way to do.

##### WRONG WAY
```html
<h4>Rental Products</h4> 
<ul class="rental">
  <li><img src="snowboard.jpg" alt="Snowboard" /></li>
</ul>
```
```css 
.rental img {
  height: 300px;
  width: 400px; 
}
```
##### RIGHT WAY
```html
<h4>Rental Products</h4> 
<ul class="rental">
  <li class="crop">
    <img src="snowboard.jpg" alt="Snowboard" />
  </li>
</ul>
```
```css 
.crop {
  height: 300px;
  width: 400px; 
  overflow: hidden;
}
```

##### Challenge
Images are currently being non-proportionally resized via CSS. Apply the `height` and `width` to their parent list items instead, and hide any `overflow`.
