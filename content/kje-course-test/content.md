
# 원(Circles) 그리고 파이(Pi)KJE

> id: intro
> section: introduction
## 들어가며

::: column.grow

인류는 하늘을 우러러보며 별과 행성, 달의 움직임을 관찰해 오며 우주의 진리를 이해하려고 노력해 왔다.

고대 그리스 천문학자들은 모든 천체가 일정한 경로를 따라 움직인다는 사실을 발견했고, 그 경로를 **궤도**라고 불렀다. 그들은 이 궤도들이 항상 원(circle)이라고 믿었고, 원은 모든 모양 중에 가장 "완벽한" 형태(모든 방향에서 대칭)였다. 결국 우리 우주의 기본 질서에서 원은 아주 걸맞는 선택이었다.

::: column(width=320)

    x-img(src="images/geocentric.jpg" width=320 height=272)

{.caption} 천동설에서 지구는 우주의 중심이다.


[계속](btn:next)

---
> id: radius
> goals: compass

[__원(Circle)__](gloss:circle) 위의 모든 점은 중심으로부터 모두 같은 거리를 가지고 있다. [컴퍼스(compass)](gloss:compass)를 사용하여 원을 그릴 수 있다.

::: column(width=320)

    x-geopad(width=320 height=300 style="position: relative;")
      svg(style="stroke-linecap: round; stroke-linejoin: round")
        circle.move(name="a" cx=160 cy=150 target="r d")
        circle.move.reveal(name="b" cx=250 cy=150 project="circle(a, 120)" target="r" when="compass")
        path.red(x="segment(a,b).contract(0.08)" target="r" arrows="both" hidden)
        path(name="c1" x="arc(a,b,1.99*pi)" hidden)
        path.blue(x="segment(b.rotate(pi/3,a),b.rotate(-2*pi/3,a)).contract(0.01)" target="d" arrows="both" hidden)
        path.green(x="arc(a,b.add(b.subtract(a).unitVector.scale(12)),1.99*pi).contract(0.02)" target="c" arrows="start" hidden)
      x-play-btn

::: column.grow

{.reveal(when="compass")} 원과 관련된 세가지 중요한 기본용어가 있다:

* {.reveal(when="compass" delay="1000")}  [{.red.b}반지름](target:r)
  은 중심으로부터 원 위의 점까지의 거리이다.
* {.reveal(when="compass" delay="3000")} [{.blue.b}지름](target:d)
  은 중심을 대칭으로 하는 원 위의 양 끝점 사이의 거리이다. 따라서 [{.blue.b}지름](target:d)의 길이는 반지름의 [[두배|반절|한배]]이다. 
* {.reveal(when="blank-0")} [{.green.b}둘레](target:c) 는 원의 가장자리를 말한다.  

:::

---
>id: similar
> goals: circle-0 circle-1 circle-2

모든 원은 [닮음](gloss:similar)이라는 중요한 특징이 있다. 평행이동하여 원의 중심을 일치시키고 적절히 반지름을 조절하면 모든 원들을 일치시킬 수 있다. 아래그림에서 [{.red}빨간색원들](target:redCircle) 을 드래그하고 반지름을 조절하여 [{.green}녹색원](target:greenCircle)에 일치시켜보라:

    figure: svg.similar-circles(width=640 height=380 viewBox="0 0 640 380")

---

## 각도(360분법과 호도법)     
>section: radians
>id: tmp

진행중
