#### Content Images
In every layout you start is important to differ between layout or content image. Each of them has best practices to be used, for content images, you should consider to use `inline` image instead of `background` some element. This will give you freedom to repeat it properly, or change origem and values properly. ex.:

##### WORST FOR CONTENT
```html
<h4>Rental Products</h4>
<ul>
  <li class="snowmobile"></li>
</ul>
```
```css
.snowmobile li {
  background: url(snowmobile.jpg); height: 300px;
  width: 400px;
}
```

##### BEST FOR CONTENT
```html
<h4>Rental Products</h4>
<ul>
  <li><img src="snowmobile.jpg" alt="Snowmobile" /></li>
</ul>
```

##### Challenge
Replace the product image incorrectly set as a background image in `<figure>` with an inline image. Use the same path and add an `alt` attribute to match the product name.
