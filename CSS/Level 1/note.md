
### CSS Note - Level 1:

#### 1. Introduction:
CSS (Cascading Style Sheets) is a style sheet language used for describing the presentation of a document written in a markup language like HTML. It defines how elements should be displayed on the screen, in print, or in other media.

#### 2. Internal Style:
Internal styles are defined within the HTML document itself using the `<style>` tag in the `<head>` section. This method is useful for small-scale styling changes within a single HTML document.

Example:
```html
<!DOCTYPE html>
<html>
<head>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
        }
        h1 {
            color: blue;
        }
    </style>
</head>
<body>
    <h1>This is a Heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

#### 3. Inline Style:
Inline styles are applied directly to individual HTML elements using the `style` attribute. This method overrides any styles applied through external or internal stylesheets.

Example:
```html
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;">This is a Heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```

#### 4. External Style:
External styles are defined in separate CSS files and linked to HTML documents using the `<link>` tag in the `<head>` section. This method allows for easy maintenance and reusability of styles across multiple HTML documents.

Example:
HTML file (index.html):
```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <h1>This is a Heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```
CSS file (styles.css):
```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
}
h1 {
    color: blue;
}
```

#### 5. Selectors:
Selectors are patterns used to select the elements you want to style. They can target elements based on their tag name, class, ID, attributes, or relationships with other elements.

#### 6. ID Selector:
ID selectors target elements based on their unique identifier specified by the `id` attribute. IDs should be unique within an HTML document.

Example:
```html
<!DOCTYPE html>
<html>
<head>
    <style>
        #main-heading {
            color: blue;
        }
    </style>
</head>
<body>
    <h1 id="main-heading">Main Heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

#### 7. Class Selector:
Class selectors target elements based on their class attribute. Classes can be applied to multiple elements, allowing for the styling of multiple elements with the same styles.

Example:
```html
<!DOCTYPE html>
<html>
<head>
    <style>
        .highlight {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <p class="highlight">This paragraph is highlighted.</p>
    <p>This is a normal paragraph.</p>
    <p class="highlight">Another highlighted paragraph.</p>
</body>
</html>
```

These are some fundamental concepts in CSS. Understanding and mastering them will give you a solid foundation for styling web pages effectively.