# helpers.css


## Intro

**helpers.css** is another [eTobb.com](http://www.eTobb.com) Open Source contribution that helps developers in three different ways:

	1. 	build websites even faster without often switching to the stylesheet and adding new selectors with the same set of rules.
	2. 	build LTR websites that can be easily converted to RTL (and vice versa).
	3. 	build websites with precise control over responsivity.


## Source

The main file that should be included is [helpers.css](https://github.com/JadJoubran/helpers.css/blob/master/src/helpers.css)  
The RTL file should be only included (after the main file) in the RTL version of your website (if any) [rtl.helpers.css](https://github.com/JadJoubran/helpers.css/blob/master/src/rtl.helpers.css)


## 1. On development speed and code maintenance

**helpers.css** allows you to use classes instead of writing styles for the most common rules (padding, margin).
How many times while writing the HTML of a view, you had to go to the css file to add a selector and write `padding-top: 5px`
Instead you can now just give the corresponding class in the html.
#### Without helpers.css
	<!-- btn btn-success are defined in Twitter bootstrap or any other button class you have defined -->
	<div class="btn btn-success header_button">Login</div>
	<style>
	.header_button{
		padding-left: 10px;
		padding-right: 10px;
		margin-bottom: 5px;
	}
	</style>

#### Using helpers.css
	<!-- btn btn-success are defined in Twitter bootstrap or any other button class you have defined -->
	<div class="btn btn-success pl10 pr10 mb5">Login</div>

If you've already used Emmet (formerly Zen Coding) you should be familiar with the class naming.


## 2. On directions (LTR/RTL)

**helpers.css** provides classes for margins, paddings, floats, text-aligns and others... 
Use those classes instead of writing the rules in your css and your website will be easily convertable to the other direction, by including th rtl.helpers.css which overrides those helpers to behave in the opposite way: .pull-left would float: right, ml5 (margin-left: 5) would do a margin-right: 5, etc..


## 3. On responsivity

**helpers.css** provides classes for fonts and line-heights.  
By using those classes you can extend the helpers.css with your own media queries to change the values of each class according to a specific viewport. [Example](https://github.com/JadJoubran/helpers.css/blob/master/examples/responsive.css)  
We understand that such responsivity can be achieved using other techniques, but it can also be achived if you're using helpers.css.


## Conventions

**helpers.css** borrows the same convention from Twitter Bootstrap: .pull-left for float: left, etc..  
And Emmet (formerly Zen Coding)  
`pr5` => `padding-right: 5px;`  
`m20` => `margin: 20px;`  
_Margin and padding helpers, values available are 0, 5, 10, 15 and 20_
_Font helpers are available from 9px to 30px(font9, font10, etc..)_
_Line height helpers are available from 10 to 30_


## But I am using a CSS Preprocessor!

**helpers.css** doesn't conflict with your CSS Preprocessor since it's letting you define your styles right from the HTML, without using inline styles of course.
You can use helpers.css with any preprocessor you want.


## Contributing

If you have ideas regarding **helpers.css**, make sure to open a new issue with descriptive details.  
Or just send me pull requests.


## Contributors

Developed by Jad Joubran [@JoubranJad](https://twitter.com/joubranjad)