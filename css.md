# CSS

|property| description|
|---|---|
|font-size|To change the font size |
|font-family|To change the family font|
|width|controls an element's width|
|border-color|Border's color|
|border-width|Border's width|
|border-style|solid (shows the border)/ |
|border-radius|Add corners to the border (with percentage 50% is the max)|
|background-color| It is what it is|
|padding|Space within the border|
|margin|Space out the border|
|color|Elements Color we add `!important` to override upon everything|

we use the `style=" color: colorName;"` to change the color.
To create a general style, we use the style tags at the top or within the `<head>` labels.

```html 
<style>
h2{
<!--We use maps to define tags styles-->
}
</style>
```

We can define **classes** within a style tags
- **class** reusable styles that can be added to HTML elements. They begin with a **.**. 


We can add multiple on sigle element with a space
```html
<style>
.class-name{ 
  <!--They also use a map syntax but to use it in as the attribute we ommit the dot "."-->
}
</style>

<h2 class='class-name1 class-name2 ...'></h2>
```
#### Add a new font family from internet

Here is an example, we need to use the `rel='stylesheet'` y  `type='text/css'` properties.
```html
<!--Place it before the style tag-->
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
```
#### Id's
They are useful to style a single element, and to modify it with a script.
- **Id** attributes should be unique. Also it has a higher relevance.
- We can style an id with css using a `#id-name{}`

A negative margin will cause the element grow.

#### Another way to select and add style, is with the attribute selector

- `[attribute = value]{}`
Ex.
```html
[type = 'radio']{
  background-color: blue;
}
```

## Absolute vs Relative
- Absolute: Physical units of length. (in , mm)
- Relative: (em, rem) relate to another length value.
  * rem: It is relative to the root font-size. 
  * em: relative to the font-size of its direct or nearest parent.
`em` example
```html
parent {
  font-size: 18px;
}
.child {
  font-size: 1.5em; <!-- Here is stablish the nearest parent font-size  (1.5 * 18) = 27-->
  padding: 2em 1em; <!-- The nearest font-size is above which is 27, so the top/bottom padding will be (2*27)=54-->
}

<div class="parent">
  <!-- I'm 15px -->
  <div class="child">
  <!-- I'm 30px, as expected -->
    <div class="child">
    <!-- I'm 60px, trouble starts! -->
      <div class="child">
 <!--     I'm 120px, now we're really in trouble!-->
      </div>
    </div>
  </div>
</div>
```
**rem** example
```html
.html {
  font-size: 16px;
}
.parent {
  font-size: 15px;
}
.child-rem {
  font-size: 2rem;
}
<div class="parent">
 <!-- I'm 15px-->
  <div class="child-rem">
  <!--I'm 32px, as expected-->
    <div class="child-rem">
    <!--I'm 32px, yep!-->
      <div class="child-rem">
      <!--I'm 32px, like clockwork!-->
      </div>
    </div>
  </div>
</div>
```

## We can create a CSS variable 
We can override them in a more specific scope, the `:root` makes the variable global.
```html
:root{
--variable-name: value;
}

h1{
  color: var(--variable-name, default);
}
```
### Media query to change a variable

We can use it to reassing a variable.
```html
 :root {
   --penguin-size: 300px;
  }
  @media (max-width: 350px) { <!-- This is the media query, before 350 the variable will be assigned black
    :root {
  --penguin-skin: black;
    }
  }
```
