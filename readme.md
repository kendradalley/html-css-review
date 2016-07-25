# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>

</body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
The img src is a self closing tag with a properties and values associated to it. The div tag is not a self closing tag and used for laying out a page.
```

---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
The first style tag is inline and added to specific tags on the HTML. Con is if you need to adjust styling you have to search line by line for it. Also unable to style multiple elements at the same time leading to more code than is necessary. Not typically recommended. Internal style sheet is still on the HTML page. Pro: all style tags are located in one section and can make multi-element changes, but still loads before the HTML, increasing load times and bounce rates.  External style sheet is best practice and is referenced in the head of the HTML page. 
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* comment like this */
div {
  border-radius: 50%; //curve the edges of the element... this will be circular
}

.header p {
  font-size: 18px; ///changes the font size of the p tag with the class of header
}

.footer { 
  position: absolute; // can be fixed to a certain position inside the parent element and not moved around by other elements
  bottom: 0; //positions the footer at the bottom of the page
}

.splash-image {
  background-image: url("../images/ocean.jpg"); //adds a image to the background of .splash-image 
  background-size: cover; //cover the entirety of the div
  width: 100%; //takes 100% of the div or container it is in
}

.ninja:hover { //when hovering over .ninja
  display: none; //this section will not be visible
  color: black; //any text associated with this class will turn black on hover
}
```


---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
