### Level 8 - Pseudo Sitzmark
Sometimes in the style to make, we'll need to attach design properties into some elements the won't in the document tree. On those cases after CSS 2.1, CSS introduces the concepts of pseudo-elements and pseudo-classes to permit formatting based on information that lies outside the document tree.

#### Pseudo Classes
Classify elements on characteristics other than their name, attributes or content; in principle characteristics that cannot be deduced from the document tree. Pseudo-classes may be dynamic, in the sense that an element may acquire or lose a pseudo-class while a user interacts with the document.

In old days, we could finish with a manual set class into the last element, so we did not need to print the bottom border of the last element. Pseudo-class solve it for us... check this up.

##### OLD DAYS
```html
<ul>
  <li><a href="#search">Search</a></li>
  <li><a href="#image">Image</a></li>
  <li class="last"><a href="#maps">Maps</a></li>
</ul>
```
```css
li {
  border-bottom: 1px solid #aaa;
}
.last {
  border-bottom: 0;
}
```

##### NEW DAYS
```html
<ul>
  <li><a href="#search">Search</a></li>
  <li><a href="#image">Image</a></li>
  <li><a href="#maps">Maps</a></li>
</ul>
```
```css
li {
  border-bottom: 1px solid #aaa;
}
li:last-child {
  border-bottom: 0;
}
```
