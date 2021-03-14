# HTML/CSS - Aula 03
[[Livros 05/06 - HTML/CSS]]

## So what is CSS, really?
```css
p {
	color: red;
}
```

```html
<link rel="stylesheet" href="styles/base.css">
```

## Anatomy of a CSS ruleset
![](HTMLCSS%20-%20Aula%2003/css-declaration-small.png)

## Selecting multiple elements

```css
p, li, h1 {
	color: red;
}
```

## Different types of selectors

```css
p { 

}

#my-id {

}

.my-class {

}

img[src] {

}

a:hover {

}
```

## Fonts and texts

```html
<head>
		<link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
</head>
```

```css
html {
  font-size: 10px; /* px means "pixels": the base font size is now 10 pixels high  */
  font-family: "Open Sans", sans-serif; /* this should be the rest of the output you got from Google fonts */
}

h1 {
  font-size: 60px;
  text-align: center;
}

p, li {
  font-size: 16px;    
  line-height: 2;
  letter-spacing: 1px;
}

```

## Boxes, boxes, it’s all about boxes
![](HTMLCSS%20-%20Aula%2003/box-model.png)

- padding
- border
- margin
 ## Changing the page color
```css
html {
  background-color: #00539F;
}
```

## Sorting the body out
```css
body {
  width: 600px;
  margin: 0 auto;
  background-color: #FF9500;
  padding: 0 20px 20px 20px;
  border: 5px solid black;
}
```

## Positioning and styling our main page title
```css
h1 {
  margin: 0;
  padding: 20px 0;    
  color: #00539F;
  text-shadow: 3px 3px 1px black;
}
```

## Centering the image
```css 

```