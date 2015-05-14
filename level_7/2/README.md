#### Hover Sprite
In a lot of cases we'll spend sometime working at transitions. To avoid tons of HTTP requests, also the need of preloading strategies, we could work with sprite images. For that:

```html
<a href="#" class="logo">Sven's Snowshoe Emporium</a>
```

```css
.logo {
  background: url(logo.png);
  display: block;
  height: 100px;
  width: 200px;
  text-indent: -9999px;
}
.logo:hover, .logo:focus {
  background-position: 0 -100px;
}
```

##### Challenge
Add the appropriate `background-position` shift to the `hover` state to make use of the new `logo2.png` sprite (see the images tab).
