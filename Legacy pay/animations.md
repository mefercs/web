# ANIMATIONS

**ANIMATION ELEMENT PROPERTIES**
- `animation-name` sets the animation name to use it in the @keyframes
- `animation-duration` animation time, remember to use `s` for seconds and `ms` for milliseconds.
- `animation-fill-mode` specifies the style applied to an element
- `animation-iteration-count:` number of animation repetitions.
- `animation-timing-function` The view of the "aceleration" we can use ease/ease-out/ease-in/linear
```css
#anim {
  animation-name:mefercs;
  animation-duration: 60s;
  animation-fill-mode: forwards; <!--Stop in 100%-->
  animation-iteration-count: 3; <!--you can also use "infinite"-->
  animation-timing-function: ease;
}
```

#### @keyframes
They are use to give css properties with `frames` from 0% - 100%

```css
@keyframes anim-name{ 
  0%{ properties }
  100%{ properties }
}
```
#### Fixed or relative positions
They allow us to use animations with offset properties.
- For example with `right`|`left`|`bottom`|`top`

####  Bezier animation function
It is use to control the animation times with the `cubic-bezier()` function. The shape of the curver represent how the animation plays out.
- The x-axis represents the animation duration.
- The y-axis represents the animation change.
Where we use p1(x1,y1) and p2(x2,y2) because p0 and p3 are the ends of the `square` (0,0) and (1,1) respectively. 
- cubic-bezier(x1, y1, x2, y2) where y1,y2,x1,x2 are >=0 and <=1.
Under the hood, p0 and p3 in combination with p1,p2 form a `line` so if we set p1 as (.25,.25) and p2(.75,.75) we create a linear function.
**The p1 and p2 can contain values bigger than 1** :()
