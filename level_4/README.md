### Level 4 - Grooming Your Code
#### DRY
In IT world DRY is an acronym for Don't Repeat Yourself. when we're talking about css, there are some places to keep it in mind. 
1. Suppose you want to include a font property in a number of text-related elements, in a not DRY way, you could finished with something like a font-family for each element h1, p also .sale. 

```html
<body>
  <div class="container">
    <h1>Sven's Snowshoe Superstore</h1>
    <p>Our snowshoes are so stylish!</p>
    <a class="sale" href="/sale">View our sales</a>
  </div>
</body>
```
##### NOT-DRY WAY
```css
h1 {
  font-family: Arial, sans-serif; 
}
p {
  font-family: Arial, sans-serif;
}
.sale {
  font-family: Arial, sans-serif;
}
```
##### DRY
###### Selector combination:
```css
h1, p, .sale {
  font-family: Arial, sans-serif; 
}
```
###### Target parent element:
```css
.container {
  font-family: Arial, sans-serif; 
}
```
