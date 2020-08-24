# 01 - Structure and Style with HTML and CSS

This is what we will make today: an app for finding and matching with people at EGGS.

![Hero image](assets/Hero.png)

Before we start, keep this in mind: HTML (and later, CSS) was first created as a document formatting language, like Word. It is also quite old. If you keep this in mind while working with HTML documents, maybe you will forgive some of the strange parts.

## HTML tags and attributes
An HTML tag / element has an opening tag and a closing tag

```html
<section>Content</section>
```

You can put elements inside other elements

```html
<section>
	<h1>Our main heading</h1>
	<p>A paragraph</p>
</section>
```

## Basic HTML document structure
Most HTML pages follow this basic structure

```html
<!DOCTYPE html>
<html>
	<head>
		[Meta data]
	</head>
	<body>
		[Content you can actually see]
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
<h1 class="huuuge">A special heading</h1>
<h1>A normal heading</h1>
<h1>A normal heading</h1>
```

Now we can target this class in our CSS file

```css
h1 {
	font-size: 200px;
	color: pink;
}

.huuuge {
	font-size: 500px;
}
```

---
## Homework
