#### Image Replacement
Sometimes we need to replace by images some elements like logos, that normally come in replace to `a` elements. On those cases we have to proceed with some steps. 
1. Add descriptive text to image-replaced elements
2. Add text-indent to hides the placeholder text

```html
  <a href="#" class="logo">Sven's Snowshoe Emporium</a>
```
```css
.logo {
  background: url(logo.png);
  display: block;
  height: 100px;
  width: 200px;
  text-ident: -9999px;
}
```

##### Challenge
The anchor in `<h1>` is now replaced with a background image, but there's no fallback text. Add the logo's text to the HTML and remove it from view.
