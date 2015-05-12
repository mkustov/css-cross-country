#### Background Images
For layout images, you should consider to use `background` some element instead of an `inline img`. This will give you security to manage it as needed. ex.:

##### WORST FOR LAYOUT
```html
<h1>Feel the rhythm, feel the rhyme, get on up, it’s bobsled time!</h1>
<img src="divider.jpg" alt="Divider" />
```

##### BEST FOR LAYOUT
```html
<h1>Feel the rhythm, feel the rhyme, get on up, it’s bobsled time!</h1>
```
```css
h1 {
  background: url(divider.jpg); margin-bottom: 10px; padding-bottom: 10px;
}
```

##### Challenge
Refactor the inline image in `.more` to be a background image, placed in the `top right` of the `.more` button.
