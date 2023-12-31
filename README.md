:root {
  --cinza: #aaa;
  --vermelha: #e93d50;
  --vermelha-escura: #af303f;
  --branca: #fff;
  --luz: rgb(229, 255, 0);
}

body {
  align-items: center;
  background: linear-gradient(45deg, #a7cfdf 0%,#23538a 100%);
  display: flex;
  justify-content: center;
  flex-direction: column;
  font-family: 'Montserrat', sans-serif;
  min-height: 100vh;
}

h1 {
  color: var(--branca);
  margin-bottom: 20px;
  font-size: 2rem;
}

.teclado {
  background: linear-gradient(to bottom, #eeeeee 0%,#cccccc 100%);
  box-shadow: 6px 8px 0 6px #666, 10px 10px 10px #000;
  border-radius: 30px;
  display: grid;
  gap: 10px;
  grid-template-columns: repeat(3, 1fr);
  padding: 10px;
}

.tecla {
  background-color: var(--branca);
  border-radius: 30px;
  box-shadow: 3px 3px 0 var(--cinza);
  color: var(--vermelha);
  cursor: pointer;
  height: 120px;
  font-size: 1.75em;
  font-weight: bold;
  line-height: 120px;
  text-align: center;
  width: 120px;
}

.tecla.ativa,
.tecla:active {
  background-color: var(--vermelha);
  border: 4px solid  var(--vermelha);
  box-shadow: 3px 3px 0 var(--vermelha-escura) inset;
  color: var(--branca);
  outline: none;
}

.tecla.focus,
.tecla:focus {
  outline: none;
  box-shadow: 1px 1px 10px var(--luz);
}

.tecla.active:focus,
.tecla:active:focus {
  box-shadow: 3px 3px 0 var(--vermelha-escura) inset, 1px 1px 10px var(--luz);
}
* {
	box-sizing: border-box;
}

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

a {
	color: inherit;
	text-decoration: none;
}

img {
	width: inherit;
}

button {
	font-family: inherit;
	font-size: inherit;
	color: inherit;
	font-weight: inherit;
	padding: 0;
	border: none;
	background-color: unset;
}

input {
	border: none;
	color: inherit;
	font-size: inherit;
	font-weight: inherit;
	font-family: inherit;
}

textarea {
	border: none;
	color: inherit;
	font-size: inherit;
	font-weight: inherit;
	font-family: inherit;
}

select {
	border: none;
	color: inherit;
	font-size: inherit;
	font-weight: inherit;
	font-family: inherit;
}
