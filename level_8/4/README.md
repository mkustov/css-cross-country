#### Pseudo Elements
Create abstractions about the document tree beyond those specified by the document language. For instance, document languages do not offer mechanisms to access the first letter or first line of an element's content. CSS pseudo-elements allow style sheet designers to refer to this otherwise inaccessible information. Pseudo-elements may also provide style sheet designers a way to assign style to content that does not exist in the source document (e.g., the :before and :after pseudo-elements give access to generated content). Ex.:

##### OLD DAYS
```html
<article>
  <p>Coffee? Hah! Our cocoa is far better.</p>
  <p>Visit from 4-5 for cocoa happy hour!&#x2744;</p>
</article>
```

##### NEW DAYS
```html
<article>
  <p>Coffee? Hah! Our cocoa is far better.</p>
  <p>Visit from 4-5 for cocoa happy hour!</p>
</article>
```
```css
article p:last-child:after {
  content: '\2744';
}
```

##### Challenge
Use a pseudo class to target the `first` paragraph, and a pseudo element to give the `first line` a `font weight` of `bold`.
