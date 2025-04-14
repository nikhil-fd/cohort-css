# CSS Cheat Sheet

### 🚩Universal selector * property
- First of all write property for universal selector i.e. * means it applies the style to all the element in the page.

  margin: 0; 
  
  removes default margin from all element.

  padding: 0; 
  
  removes default padding from all element. 

  box-sizing: border-box; 

  changes default box-model so that width and height include padding and border, rather than adding them on top of the specified dimension.

```CSS
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
### 🚩How to set perfect property for "color" & "background-color"
- Always write color/background-color in hexadecimal so that exact color will apply in browser, if we give color: red with name then browser convert it to hexa and it looses some color quality.
```css
color: #212121;
background-color: #ff0000;
```
### 🚩when use `<img>` element must use a property i.e.
```css
img{
    object-fit: cover;
}
``` 
### 🚩when we give width: 100vw; & height: 100vh; to a &lt;div&gt; then automatically horizontal and vertical scrollbar will appear. So how to remove/disappear this horizontal & vertical scroll bar?
```css
  1st need to set universal selector(*)
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  div{
    width: 100vw;
    height: 100vh;
  }
```
### 🚩how to make button clickable using vanilla css?
```css
button{
    color: #d9b40f;
    padding: 10px;
    background-color: #523f36;
    border: none;
    border-radius: 10px;
    padding: 15px;
    margin: 35px 5px;
    cursor: pointer;
    box-shadow: 0 4px 0 #523f36;
    transition: all 0.15s ease-in-out;
}
button:hover{
    background-color: #523f36;
    transform: translateY(-2px);
    box-shadow: 0 4px 0 #523f36;
}
button:active{
    transform: translateY(2px);
    box-shadow: 0 1px 0 #523f36;
}
```
### 🚩How to give shadow in 4 side such as button, div box, span box etc?
```css
box-shadow: 0 0 5px 2px #ffffff;
```
- When give shadow in 4 side then keep horizontal = 0 & vertical = 0
- horizontal = 0
- vertical = 0
- blur = 5px
- stretch = 2px
- color = #ffffff