# AC 
Semantic meaning: means that the tag you use describe the information contained.
- A web page should only contain only a `<h1></h1>` tag.
## Main structure tags
- `<main></>` it should wrap the page content, and there is a single main tag per page.
- `<header></>` For introductory content. It's placed within the body tag.
- `<footer></>` It's at the bottom page that contains copyright info or links.
- `<nav></>` for easy screen navigation (navigation var).
- `<article></>` It is used to section independent and self-contained content.
- `<section></>` Similar with `<article>` but this tag have thematically content.
- `<div></>` Groups content.
- `<audio alt="" controls></>` has a control attribute, it contains a `<source src="" type="">` tag.
- `<figure></>` it contains `<figcaption>`, they both wrap visual representation(image, chart, diagram)
- `<label></>` wraps the text for a specific form control item.
- `<fieldset></>` wrap radio buttons whithin the `<form>` which contains a `<lengend>` tag( supplying the `<p>` tag ).-
- `<input type="date">` which give us a date picker.
For example if a book is the article, each chapter is a section.
- `<time datetime="00-00-00></>"` which is used to standarize times.
* In anchor tags use descriptive text for screen users.
* `accesskey="letter" attibute available in any HTML element, useful for keyboard-only users.`
* `tabindex="number"` indicates an element can be focused on.
When we use tabindex >= 1, will modify the normal flow, we'll tab from 1,2,3,k and then we'll continue with tabindex="0" that are set by default.
```css
<!-- When tabindex is selected, element:focus is activated.
```
<img src="https://imgs.search.brave.com/B0_kgD7shsqTSUMLPCaXUTrLOVFBIJd8dhA4a7wlaVw/rs:fit:1024:768:1/g:ce/aHR0cHM6Ly9zMy5h/bWF6b25hd3MuY29t/L3Zpa2luZ19lZHVj/YXRpb24vd2ViX2Rl/dmVsb3BtZW50L3dl/Yl9hcHBfZW5nL2h0/bWw1X3NlY3Rpb25p/bmdfaGlnaF9sZXZl/bC5qcGc" alt="STRUCTURE HTML TAGS">

## Hide content meant for screen readers with css
```css
.sr-only {
  position: absolute;
  left: -10000px;
  width: 1px;
  height: 1px;
  top: auto;
  overflow: hidden;
}
```
