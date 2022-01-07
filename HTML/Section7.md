# Section 7: The World of CSS selectors

#### Universal selector
```css
* {
  color: black;
}
```

#### Element selector
```css
button {
  color: black;
}
```

#### Selector lists
```css
h1,h2 {
  color: black;
}
```
#### ID selector
id can be used only once in the same `html` file
```css
#id {
  color: black;
}
```
#### Class selector
```css
.class {
  color: black;
}
```
#### Descendant selector
```css
.section a {
  color: black;
}

footer a {
  color: red;
}
```
#### Direct child selector
```css
.class > a {
  color: black;
}
```
#### Attribute selector
```css
input[type="text"] {
  color: pink;
}
```
#### Pseudo classes
```css
a:hover {
  color: orange;
}

div:nth-of-type(2n-1) {
  background-color: red;
}
```
#### Pseudo element
Indicates a specific part of a seletor
```css
selector::after {
  content: "This is a pseudo element";
}
```
#### CSS Cascade
Order of CSS matters <br>
The latest CSS will be applied

#### CSS Specificity
It is a measure of how specific a given selector is. The more specific selector "wins"<br>
`!important` > style attribute > `ID` > `CLASS` > `ELEMENT` <br>
![alt text](https://i2.wp.com/css-tricks.com/wp-content/uploads/2021/01/cssspecificity-calc-1_kqzhog.png?w=570&ssl=1)

