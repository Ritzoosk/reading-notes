# 14 A
## perfect team
- 
## CSS Transform
- transform Syntax
>div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

- 2d rotation
>.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

- transform: scale(.75)
  - you cant scale (x, y)

- translateX
>.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

- skew
>.box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
}

- combind
>.box-1 {
  transform: rotate(25deg) scale(.75);
}
.box-2 {
  transform: skew(10deg, 20deg) translateX(20px);
}

- cube
>HTML: <div class="cube">
  <figure class="side top">1</figure>
  <figure class="side left">2</figure>
  <figure class="side right">3</figure>
</div>


- CSS:
>.cube {
  position: relative;
}
.side {
  height: 95px;
  position: absolute;
  width: 95px;
}
.top {
  background: #9acc53;
  transform: rotate(-45deg) skew(15deg, 15deg);
}
.left {
  background: #8ec63f;
  transform: rotate(15deg) skew(15deg, 15deg) translate(-50%, 100%);
}
.right {
  background: #80b239;
  transform: rotate(-15deg) skew(-15deg, -15deg) translate(50%, 100%);
}

- perspective
>.box {
  transform: perspective(200px) rotateX(45deg);
}

- perspective origin
>.original {
  perspective: 200px;
}
.box {
  transform: rotateX(45deg);
}
.original-1 {
  perspective-origin: 0 0;
}
.original-2 {
  perspective-origin: 75% 75%;
}
.original-3 {
  perspective-origin: 20px 40px;
}

- 3D transforms
>.box-1 {
  transform: perspective(200px) rotateX(45deg);
}
.box-2 {
  transform: perspective(200px) rotateY(45deg);
}
.box-3 {
  transform: perspective(200px) rotateZ(45deg);
}

# 14b
- social sensitivity
- equality in distribution of conversational turn-taking
- less fear of rejection
- establish psychologically safe environments
- 