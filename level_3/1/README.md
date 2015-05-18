#### Box Model
When adapting a layout is important to have in mind the box model. Each DOM element has a imaginary diagram with 4 areas (content area, padding area, border area and margin area). 

Total calculated box width = content width + padding width + border width;

ex.: 100px content width + 15px padding width + 10px border width = 125px box width
```css
.downhill {
  border: 5px solid #fff;
  padding-left: 10px;
  padding-right: 5px;
  width: 100px;
}
```
##### Challenge
The `<figure>` in our page footer should have a total box `width` of `180px`. Add an appropriate content `width` given its base `padding` and `border`.
