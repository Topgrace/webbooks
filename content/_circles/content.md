# Circles and Pi

## IntroductionKJE한글k

> section: introduction
> id: intro
> trailer: tBJUNvCBkLo
> color: "#5A49C9"
> level: Intermediate
> next: graph-theory

::: column.grow

For as long as humans have existed, we have looked to the sky and tried to explain life on Earth
using the motion of stars, planets and the moon.

Ancient Greek astronomers were the first to discover that all celestial objects
move on regular paths, called __orbits__. They believed that these orbits are
always circular. After all, circles are the “most perfect” of all shapes:
symmetric in every direction, and thus a fitting choice for the underlying
order of our universe.

::: column(width=320)

    x-img(src="images/geocentric.jpg" width=320 height=272)

{.caption} Earth is at the center of the _Ptolemaic universe_.

:::

---
> id: radius
> goals: compass

Every kje point on a [__circle__](gloss:circle) has the same distance from its
center. This means that they can be drawn using a [compass](gloss:compass):

<!-- circle.move(name="a" cx=160 cy=150 target="r d")
        circle.move.reveal(name="b" cx=250 cy=240 project="circle(a, 120)" target="r" when="compass")
        path.red(x="segment(a,b).contract(0.08)" target="r" arrows="both" hidden)
        path(name="c1" x="arc(a,b,1.99*pi)" hidden)
        path.blue(x="segment(b.rotate(pi/3,a),b.rotate(-2*pi/3,a)).contract(0.01)" target="d" arrows="both" hidden)
        path.green(x="arc(a,b.add(b.subtract(a).unitVector.scale(12)),1.99*pi).contract(0.02)" target="c" arrows="start" hidden) -->

::: column(width=320)

    x-geopad(width=320 height=300 style="position: relative;")
      svg(style="stroke-linecap: round; stroke-linejoin: round")
        circle.move(name="a" cx=160 cy=150 target="r d")
      x-play-btn

::: column.grow

{.reveal(when="compass")} There are three important measurements related to
circles that you need to know:

* {.reveal(when="compass" delay="1000")} The [{.red.b}radius](target:r)
  is the distance from the center of a circle to its outer rim.
* {.reveal(when="compass" delay="4000")} The [{.blue.b}diameter](target:d)
  is the distance between two opposite points on a circle. It goes through its
  center, and its length is [[twice|half|the same as]] the radius.
* {.reveal(when="blank-0")} The [{.green.b}circumference](target:c)
  (or perimeter) is the distance around a circle.



