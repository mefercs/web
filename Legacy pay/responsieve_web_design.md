# Responsive Web Design Principles
## Create a media Query
They consists on media types(Which can match the type of a device).
- We can select the `width` or the `height`
```css
<!-- Device with width < 100px, returns the css when the maximum size is 100px-->
@media (max-width: 100px) {
  ...content
}

<!-- Device with width > 300px, returns the css when the minimum size is 200px-->
@media (min-width: 200px) {
  ...content
}
```
---
## Responsive Image
```css
img {
  max-width: 100%; <!-- The image never will be greater than the container where is contained-->
  height: auto; <!-- This keeps the essence of the image-->
}
```
---
## Use a Retina Image for Higher Resolution Displays
- **PPI** : Pixels Per Inch : Which measures the pixels density on the device screen, which is different on each device.
- **DPI** : Dots Per Inch
- To solve the quality lack in high-resolution devices we use the half of the image dimensions.
---
## Responsive Typography
- We can use a another relavite measurement unit called viewport, they are 4 main units: 
  * vw : viewport width : 10vw == 10% of the viewport's width
  * vh : viewport heightt : 10vw == 10% of the viewport's height
  * vmin : viewport minimum : 70vmin == 70% of the minimum viewport ( between height or width viewport )
  * vmax : viewport maximum : 10vmax == 10% of the maximum viewport 
