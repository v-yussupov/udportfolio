GitHub Pages link:
http://v-yussupov.github.io/udportfolio/

Optimization actions:

1. List of technics to achieve sufficient PageSpeed Insights score<br>
	1.1 Optimized CSS - removed unnecessary lines, divided it in two parts - critical and non-critical,	minified critical part (I included full version for examination: css/2minify.css) and inlined it<br>
	1.2 Non-critical part (style.css) is loaded after initial painting of the page via minified JS at the end of the body tag<br>
	1.3 Defined font-family with @font-face within above stated critical part of CSS (placing it within non-critical part will result in slight increase of performance and flash of unstyled text)<br>
	1.4 Used media="print" for print.css<br>
	1.5 Used async for Google Analytics script<br>
	1.6 Placed performance and analytics scripts at the end of the body tag<br>
	1.7 Specified actual images dimensions<br>
	1.8 Optimized images quality<br>
	1.9 Replaced large pizzeria.jpg with pizzeria-small.jpg<br>
	1.10 Tried lazy image loading (link 13), but decided not to use it due to insignificant difference<br>

2. List of technics to optimize pizza-page<br>
	2.1 Optimized images<br>
	2.2 Refactor main.js (comments on changes are included in main.js):<br>
		2.2.1 Changed bootstrap style to include small screens and reduce proportion of the image div<br>
		2.2.2 Removed variables declaration from the cycle of changePizzaSizes(size)<br>
		2.2.3 Removed variables declaration from the pizza adding cycle, used function addPizza() to append all pizzas once as a DocumentFragment<br>
		2.2.4 Declared variables outside updatePositions() and defined some of them when the document is loaded<br>
		2.2.5 Defined scrollTop outside of the cycle of updatePositions()<br>
		2.2.6 Used DocumentFragment to append background pizzas<br>
		2.2.7 Changed calculation of visible background pizzas quantity<br> 	
	
List of links:

1. stackoverflow.com
2. developer.mozilla.org
3. w3schools.com
4. https://gongled.ru/all/web-pages-optimization/
5. http://www.port80software.com/support/articles/developforperformance1.asp
6. http://www.bookofspeed.com/index.html
7. PageSpeed Insights Chrome plugin 
8. http://cssminifier.com/ - minify CSS
9. http://jscompress.com/ - minify JavaScript
10. https://tinypng.com/ - optimize PNG
11. https://kraken.io/web-interface - optimize JPG
12. Search results from google.com on different related topics
13. http://toddmotto.com/echo-js-simple-javascript-image-lazy-loading/