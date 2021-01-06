# CSS NOTES

CH 10 pg 226
- <p>, <i>, <a>  elements
- Associate element <p>  p{font-family: Arial;} 
- p=selector      {}=Declaration
- Declarations can add properties and values
- html can be externally linked to CSS file that styles it
- href specifies path
- `<link href="css/styles.css" type="text/css"
 rel="stylesheet" />`
- `<style>` `<style type="text/css">`
- specifies?

## Selectors
![csssel](https://lh3.googleusercontent.com/NDX-rObVlI6MAm13WeRs9WIe0taOPh_ELtcD-oUMJaFig97bn76DyRHNguOVKTsD-6XPQDTNak_d5aUjP4xqifVtV9SuL8I-uQMfVYvbd4PV8m0F65Xf2mNGPOff7B28d8WNSwzx54R3l9I7FK-yWCJWlAKHJi0pgIlewsyOMdCcndcFD52WAYnlaCnB-VwSTtcKAF3ZiAGEYGWVrYRBzyoLoVisSkd9ZynpaE-AYrZL3-o1exDcmpMhNkmFW_tOdcpHdXO6om2mq8GEkpDq893bkcu3gyI4nElStkBbdX9SzHeG_yUOhi_j0TKjGR5T-htR3Asoix4nXgEpHwmNCzBrJ4LAnOyGvK6uGtuoh97kpk_YOZLKC29R7VqstSOddyn16qdiorTMhGrOEfYyuDZW-LNaWNwyq8wVP6RSFpavsy2GgR56Xs8yfZkMYxI5Fc2IYgeboyA9xHHL3-YaesvDSUcpcc5HxxVr8J8Zy6lPku9mAVSh9JNVc16EfF0NkJBPjDf23QOwrRFgboZ-lusprnRapRZflCCR8p8kYAVzJ31Nz1UOQMgHIeTL10gymnP5m63hrxcIXq8fgiL8a63oARRkaSwOoa4-OsZGlB4lcB56xZsRw8_Aldrae6S_H7XsniRNEWg_vAjwmNHWnTdSZY0xvcqeZ7lx49LERrYsYPZHQb2gmDFAIc_SkQ=w322-h382-no?authuser=0)

# Colors ch11 pg 247 pdf 245
- specify via RBG
  - rgb(100,100,90)
- Hex
  - For example: #ee3e80
- Color names
  - DarkCyan

### background color
> body {
background-color: rgb(200,200,200);}
h1 {
background-color: DarkCyan;}
h2 {
background-color: #ee3e80;}
p {
background-color: white;}

- RGB (102,205,170) (red,grn,blu) (###,###,###)
- HEX  #66cdaa 66=102red, cd=105grn, aa=170blu 

### Opacity
- The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).
> p.one {
background-color: rgb(0,0,0);
opacity: 0.5;}
p.two {
background-color: rgb(0,0,0);
background-color: rgba(0,0,0,0.5);}

- RGBA
- HSL color, Hue, Saturation, Lightsness
- CSS3: HSL & HSLA

> <title>Color</title>
 <style type="text/css">
 body {
 background-color: silver;
 color: white;
 padding: 20px;
 font-family: Arial, Verdana, sans-serif;}
 h1 {
 background-color: #ffffff;
 background-color: hsla(0,100%,100%,0.5);
 color: #64645A;
 padding: inherit;}
 p {
 padding: 5px;
 margin: 0px;}
 p.zero {
 background-color: rgb(238,62,128);}
 p.one {
 background-color: rgb(244,90,139);}
 p.two {
 background-color: rgb(243,106,152);}
 p.three {
 background-color: rgb(244,123,166);}
 p.four {
 background-color: rgb(245,140,178);}
 p.five {
 background-color: rgb(246,159,192);}
 p.six {
 background-color: rgb(245,176,204);}
 p.seven {
 background-color: rgb(0,187,136);}
 p.eight {
 background-color: rgb(140,202,242);}
 p.nine {
 background-color: rgb(114,193,240);}
COLOR 260
Example
COLOR
 p.ten {
 background-color: rgb(84,182,237);}
 p.eleven {
 background-color: rgb(48,170,233);}
 p.twelve {
 background-color: rgb(0,160,230);}
 p.thirteen {
 background-color: rgb(0,149,226);}
 p.fourteen {
 background-color: rgb(0,136,221);}
 </style>
</head>
<body>
 <h1>pH Scale</h1>
 <p class="fourteen">14.0 VERY ALKALINE</p>
 <p class="thirteen">13.0</p>
 <p class="twelve">12.0</p>
 <p class="eleven">11.0</p>
 <p class="ten">10.0</p>
 <p class="nine">9.0</p>
 <p class="eight">8.0</p>
 <p class="seven">7.0 NEUTRAL</p>
 <p class="six">6.0</p>
 <p class="five">5.0</p>
 <p class="four">4.0</p>
 <p class="three">3.0</p>
 <p class="two">2.0</p>
 <p class="one">1.0</p>
 <p class="zero">0.0 VERY ACID<

