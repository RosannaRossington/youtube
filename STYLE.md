CSS

Setting a static width and height on an element poses a problem for any type of fluid/flexible design. If the parent area shrinks in width to be narrower than the video, the video will break out, not shrink to fit.
The idea is to create a box with the proper ratio (4:3, 16:9, etc.), then make the video inside that box stretch to fit the dimensions of the box.

border-style: dotted works as long as your border is no larger than a pixel or two. It then become a square and the bigger the border the bigger the square.

Chrome and Safari apparently these browsers need explicit `border-style` and `border-color` properties. Code has been updated with the fix.