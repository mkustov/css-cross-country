#### Collapsing Margins
Margin properties specify the width of the margin area of a box. In a page with 3 main areas (header, article and aside), where your layout requests a margin of 20px between them, you could end up with something like:
```html
<header>
</header>
<article>
</article>
<aside>
</aside>
```

```css
article {
  margin: 20px 0; 
}
```
Now think about a layout change, we want to remove the article, leaving header and aside with a 20px margin between them... it shouldn't work now? Is it? A proper way to do that will be think about them as complementary blocks with a first margin added to the second with a total of 20px... **BUT THIS IS WRONG - in most cases*.

According to w3c spec, two adjoining margins will be collapse and the highest value of them will be the final margin between those blocks. For example, with the following style definition the margin between header and article should be 20px and between article and aside will be 30px.

```css
header {
  margin: 20px 0; 
}
article {
  margin: 10px 0;
}
aside {
  margin: 30px 0;
}
```
