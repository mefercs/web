# html cheatsheet

```html
<!--We can send html with the form tag-->
<form action="url-to-send">
  ...tag  
</form>

<!--create a submit button, we can add it to the form tag-->
<button type="submit"> a button </button>

<!--within a input element we can add the `required` attribute-->
<input type="text" placeholder="ex-text-to-show" required>
```

To create a radio button for one multiple answer 

```html
<label for="option">
  <input id="option "type="radio" name="some-group"> message
</label>

<input id="option" type="radio" name="some-group">
<label for="option">message</label>
<!--To create a default checked radio button we need to add the 'checked' attribute on the input tag-->
```
#### SO important tags
```html
<div></div>

<!DOCTYPE html-version- > 
```
Use checkboxes
```html
<!--It's similar as radio buttons-->
<label>
  <input type='checkbox' name='group-name'>My checkbox
</label>
<!--To create a default checked checkbox we need to add the 'checked' attribute on the input tag-->
```
We need to add the `value="value"` property to the input radio,buttons, and checkboxes
```html
<label for="indoor">
  <input id="indoor" value="indoor" type="radio" name="indoor-outdoor">Indoor
</label>
<label for="outdoor">
  <input id="outdoor" value="outdoor" type="radio" name="indoor-outdoor">Outdoor
</label>
<!--If we set the indoor radio button, then the send data is `indoor-outdoor=indoor`-->
<!--By default the value if not set, is 'on'-->
```
## html page structure tag

```html
<!DOCTYPE html>
<html>
<!--your html code-->
</html> 
```

# Head and body of the page
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Example title</title>
  </head>
  <body>
    <div>
    </div>
  </body>
</html>
```
