#### Proportional Image Crop
To proportionaly crop image, you should choose one of the containers size to be equal (`width` or `height`) and use the other as auto.

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
.crop img {
  height: 300px;
  width: auto;
}
```

##### Challenge
Now our images aren't squished, but they don't use the container effectively. Set a `height` on the images to match the container and make sure the `width` scales proportionally automatically.
