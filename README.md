GitHub Pages link:
http://v-yussupov.github.io/udportfolio/

Optimization actions:

1. List of technics to achieve sufficient PageSpeed Insights score 
	1.1 Optimized CSS - removed unnecessary lines, divided it in two parts - critical and non-critical,	minified critical part (I included full version for examination: css/2minify.css) and inlined it
	1.2 Non-critical part (style.css) is loaded after initial painting of the page via minified JS at the end of the <body>
	1.3 Defined font-family with @font-face within above stated critical part of CSS (placing it within non-critical part will result in slight increase of performance and flash of unstyled text)
	1.4 Used media="print" for print.css
	1.5 Used async for Google Analytics script
	1.6 Placed performance and analytics scripts at the end of the <body>
	1.7 Specified actual images dimensions
	1.8 Optimized images quality
	1.9 Replaced large pizzeria.jpg with pizzeria-small.jpg
	1.10 Tried lazy image loading (link 13), but decided not to use it due to insignificant difference

2. List of technics to optimize pizza-page
	2.1 Optimized images
	2.2 Refactor main.js (comments on changes are included)
	
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
13. http://toddmotto.com/echo-js-simple-javascript-image-lazy-loading/ - simple JS lazy image loading