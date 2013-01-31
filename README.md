CSS-Hacks
=========

This repository is to collection of every browser-specific css selector and style attribute hack I've seen.


**Selector Hacks:**


```css
/* IE6 and below */
* html #idname  { background: red; }

/* IE7 */
*:first-child+html #dos { color: red }

 
/* IE7, FF, Saf, Opera  */
html>body #tres { color: red }
 
/* IE8, FF, Saf, Opera (Everything but IE 6,7) */
html>/**/body #cuatro { color: red }
 
/* Opera 9.27 and below, safari 2 */
html:first-child #cinco { color: red }
 
/* Safari 2-3 */
html[xmlns*=""] body:last-child #seis { color: red }
 
/* safari 3+, chrome 1+, opera9+, ff 3.5+ */
body:nth-of-type(1) #siete { color: red }
 
/* safari 3+, chrome 1+, opera9+, ff 3.5+ */
body:first-of-type #ocho {  color: red }
 
/* saf3+, chrome1+ */
@media screen and (-webkit-min-device-pixel-ratio:0) {
 #diez  { color: red  }
}
 
/* iPhone / mobile webkit */
@media screen and (max-device-width: 480px) {
 #veintiseis { color: red  }
}
 
 
/* Safari 2 - 3.1 */
html[xmlns*=""]:root #trece  { color: red  }
 
/* Safari 2 - 3.1, Opera 9.25 */
*|html[xmlns*=""] #catorce { color: red  }
 
/* Everything but IE6-8 */
:root *> #quince { color: red  }
 
/* IE7 */
*+html #dieciocho {  color: red }
 
/* IE 10+ */
@media screen and (-ms-high-contrast: active), (-ms-high-contrast: none) {
   #veintiun { color: red; }
}
 
/* Firefox only. 1+ */
#veinticuatro,  x:-moz-any-link  { color: red }
 
/* Firefox 3.0+ */
#veinticinco,  x:-moz-any-link, x:default  { color: red  }
 
/* FF 3.5+ */
body:not(:-moz-handler-blocked) #cuarenta { color: red; }
```

**Attributes**

```css
/* Underscore to target - IE6 */
#once { _color: blue }
 
/* Asterisk to target - IE6, IE7 */
#doce { *color: blue; /* or #color: blue */ }
 
/* Everything but IE6 */
#diecisiete { color/**/: blue }
 
/* IE6, IE7, IE8, but also IE9 in some cases :( */
#diecinueve { color: blue\9; }
 
/* IE7, IE8 */
#veinte { color/*\**/: blue\9; }
 
/* IE6, IE7 -- acts as an !important */
#veintesiete { color: blue !ie; } /* string after ! can be anything */
 
/* IE8, IE9 */
#anotherone  {color: blue\0/;} /* must go at the END of all rules */
 
/* IE9, IE10 */
@media screen and (min-width:0\0) {
    #veintidos { color: red}
}
```

Thanks to Paul Irish for the Select and Attribute list.

More to be updated, Stay tuned!
