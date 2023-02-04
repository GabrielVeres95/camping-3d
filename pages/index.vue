<template lang="pug">
.full-screen
  .logo 
    img(src='~/assets/camper_old.svg')
  iframe(src='https://my.spline.design/carcampingphysicscopy-7d72a1efc344d683920c74b8e424b28e/' frameborder='0' width='100%' height='100%')
  .instructions Use W,A,S,D to play*
</template>

<style>
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}
body {
	line-height: 1;
}
ol, ul {
	list-style: none;
}
blockquote, q {
	quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}
table {
	border-collapse: collapse;
	border-spacing: 0;
}

.full-screen {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
}

.logo {
  position: absolute;
  left: 50%;
  top: 30px;
  transform: translateX(-50%);
  width: 20rem;
}

.logo img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.instructions {
  position: absolute;
  bottom: 60px;
  left: 50px;
  display: none;
  font-size: 18px;
  font-family: 'Verdana', sans-serif;
  font-weight: bold;
  color:darkgreen;
}

@media (min-width: 1400px) {
  .instructions {
    display: inline-block;
  }
}

</style>

<script>
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'
})
