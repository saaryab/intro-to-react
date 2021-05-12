## Web Pages

### HTML

HTML is the basic markup browsers use to display documents:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body class="news-feed-page">
    <h1>News feed</h1>
    <div class="article">
        <div class="title">Some Great News</div>
        <div class="date">April 25, 2021</div>
        <div class="author">Joe Brody</div>
    </div>
  </body>
</html>
```
### CSS

CSS is a stylesheet used to reference HTML elements and define their style.
SCSS/SASS is used to add functionality to the CSS language

```scss
.news-feed-page {
  h1 {
    font-size: 2rem;
  }
  .article {
    .title {
      text-transform: uppercase;
      font-weight: bold;
    }
    .date {
      color: darkslategray;
    }
    .author {
      color: darkslategray;
      font-style: italic;
    }
  }
}
```

### JavaScript

JavaScript is a scripting language that the browser can run.
It is limited in access to the host system by the browser, but it can access
the DOM (HTML elements) as well as various browser APIs like location.

An example of JavaScript interacting with the DOM:
```javascript
<div id="title">Some News<div>
<button
    onclick='document.getElementById("title").innerHTML = "Some Great News"'>
    Make it Better
</button>
```
A plain JavaScript function:
```javascript
<script>
    function factorial(num) {
        if (num < 0) return -1; // invalid input
        if (num === 0) return 1;
        return num * factorial(num - 1);
    }
    
    const myFactorial = factorial(5);
    console.log(myFactorial);
</script>
```