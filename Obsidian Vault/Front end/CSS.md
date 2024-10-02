
# chapter 1
- external stylesheet
- internal style seet
- inline stylesheet
- rule set of css MDN
	- anatomy of css rule set
- w3c style validation service

# chapter 2

- selectors
- 3 types of selector
	1. element selector
		- body selectors
			- inheritance
		- paragraph selector
	2. class selectors 
		- access using . opearot
		- stronger than element selector
	3. id selector
		- id present one time in html
		- not good practice to use in CSS
- group selectors
	- h1, h2 {   }
- element inside element
	- p span {   }
	- for this use class it is good practice
- universal selectors
	- *
	- css reset
- stylesheet acts like waterfall
	- last will be applied
	- use inspect to debug what rule overwrite which one
- inheritance
	- borders does not have inheritance
	- form elements does not inheritance
- practices
	- html
	- body
	- main
**summary**
hirercy of selector
- element selector
- class selector
- id selector
- important - do not use it
#### specifity calculator

# chapter 3 - colors
- backgroud color
	- 140 color names
- font color
- rgb - max value is 255 - black is 000 white is 255,255, 255
- rgba - a alpha channel- 0 - to 1
	- alpha chaneel
	- 0 to 1
	- 0 is normal
	- 1 is transparent
- hexadecimal - like rgb
	- start with #
	- 0 to 9
	- a to f
	- 0 is the black
	- f is white (active)
- hsl - and hsla in percent
- hue, saturation and light and alpha
- hue is 360
- ### tools
	- coolors -
		- color pallete picking tool
		- contrast checker
# chapter 4 - units & sizes
- we use pixels as units
- 1px - 1/96 of inch per MDN
- default font-size is 16px
- width is block level element
- relative units
	- rem  - used for font size
		- 1 rem is default
		- rem - root
		- if we put 2rem it will double
	- em
		- if we have **main as 2rem**
		- and use **p as** **2em** p will double from main
	- ch - characters
		- used with width 
		- 40 characters per line
	- vw - viewport width
		- use percent for eliminate horizontal bar
	- vh - viewport height
		- 
- user agent stylesheet
	- cannot override this
- ## summary
- font-size - px
- relative units
	- rem
	- em
	- ch
	- vw
	- vh
# chapter 5 - Box model
- everything is box model
-  insde computed, there is a model
- padding is inside of a border
- em responds with font size of element
- this is order of style in element
	- content
	- padding
	- border
	- margin
- to take the control of all element margin and padding, need to use reset seletor with margin and padding 0
- ### css arsg
	- margin
	- padding
	- outline
	- outline-offset
	- border-radius
- # chapter 5 - typography - text arranged and presented
	- input, button 
		- font inherit
	- text decoration - underline
	- text-transform - lowercase
	- text-align
	- text-indent
	- line-height
	- letter-spacing
	- word-spacing
	- font-weight- 100, lighter, bolder
	- font-style - italic
	- font-family - can use choice wise, seperated by comma
	- select from google import text from google to css file directly
- # chapter 6 - styling links
	- anchor tags
	- anchor tags with psudocode class
		- visited
		- hover
		- active