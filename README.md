<h1>css-grid</h1>
<h2>HI there!</h2>
This an simple example of how to use css grid functions that i made for studying purposes,
i hope it help you too!
and you can test it on code pen by this <a href="https://codepen.io/brunodhein/pen/vYYGqqq">link</a>

Or you can take a look at it down there:
<h4>HTML</h4>
```html
<!--an simple gride example by: Bruno Dhein-->
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <link rel="stylesheet" href="css/global.css" />
    <link rel="stylesheet" href="css/reset.css" />
  </head>

  <body>
    <div class="container">
      <header>HEADER</header>
      <main>MAIN</main>
      <div id="test">RANDOM DIV</div>
      <div id="test2">RANDOM DIV 2</div>
      <div id="test3">RANDOM DIV 3</div>
      <footer>FOOTER</footer>
    </div>
  </body>
</html>
```

<h4>CSS</h4>

```css
/* an simple gride example by: Bruno Dhein*/
body {
  font-size: 20px;

  color: rgb(128, 0, 0);
}
/* the grid-area atributte changes the position on the grid */
header {
  background: rgb(1, 41, 4);
  grid-area: h;
}

main {
  background: rgb(81, 82, 16);
  grid-area: a;
}
footer {
  background: #000000;
  grid-area: f;
}
#test {
  background: #fcdd79;
  grid-area: t;
}
#test2 {
  background: #ebdaa4;
  grid-area: s;
}
#test3 {
  background: #1100ff;
  grid-area: y;
}
/*  try some other combinations to see what it does
    "a h h"
    "s s t"
    "y y y"
    "f f f"
    
    "f f f"
    "a s t"
    "y y y"
    "h h h"
    
    "h h t"
    "a s t"
    "y y y"
    "f f f"
    
    and use your imagination*/
/*     1 "h h h"  each set of cordinates (like "h h h") represents an row and each cordinate (like "h") represents an column
       2 "a s t"
       3 "y y y"
       3 "f f f"     */
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 150px 70vh 10vh 20vh; /* 100vh represents the whole page so each 1vh it's one part of the page and so on */
  grid-template-areas:
    "h h h"
    "a s t"
    "y y y"
    "f f f";
  margin: 0 100px 0 100px;
  font-family: "Arial", sans-serif;
  font-weight: bold;
}

```
