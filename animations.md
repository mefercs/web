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
It is use to control the animation times with the `cubic-bezier()` function.

