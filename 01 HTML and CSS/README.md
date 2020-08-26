# 01 - Structure and Style with HTML and CSS

This is what we will make today: an app for finding and matching with people at EGGS. I've made a [proposal](https://codesandbox.io/s/kinderapp-jog8u?file=/index.html) for how to code this, which you can check out if you get stuck along the way.

![Hero image](assets/Hero.png)

Before we start, know this: HTML (and later, CSS) was first created as a document formatting language, like Word. It is also quite old. If you keep this in mind while working with HTML documents, maybe you will forgive some of the strange parts.

## HTML tags and attributes
An HTML tag / element has an opening tag and a closing tag

```html
<section>
...content goes here
</section>
```

You can put elements inside other elements

```html
<section>
	<h1>Kinder</h1>

	<h2>Alexander, 29</h2>
	<p>I like long walks on the beach and late nights by the fireplace</p>
</section>
```

## Basic HTML document structure
Most HTML pages follow this basic structure

```html
<!DOCTYPE html>
<html>
	<head>
		...meta data
	</head>
	<body>
		...content you can actually see
	</body>
</html>
```

## Adding stylesheets (css)
The standard way of styling html documents is to add a separate style document that describes what our html elements should look like. 

As an example, lets give our `<h1>` heading elements a black bottom line.

```css
h1 {
	border-bottom: 1px solid black;
}
```


## Targeting styles with classes and ids
However, that css rule will make EVERY `<h1>` element in our html document get the same style. What if we only want to style ONE of our heading elements?

Let's add a specific identifier to one of our heading elements, to make that stand out even more.

```html
<h1>A normal heading</h1>

<h1 class="special-heading">A special heading</h1>

<h1>A normal heading</h1>

<h1>A normal heading</h1>
```

```css
/* Selector: all h1 elements */

h1 { 
	font-size: 200px;
}


/* Selector: all elements with the class "special-heading" */

.special-heading {
	font-size: 500px;
	color: pink;
}
```
---
## Task
Your mission, should you choose to accept it, is to develop the rest of the Kinder app.

---
## Homework and extra resources
* Mozilla Developers Network (your go-to encyclopedia of web stuff)
	* MDN page for [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
	* MDN page for [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [Fireship on YouTube](https://www.youtube.com/c/AngularFirebase/featured) (really good video tutorials, both easy and advanced topics)
