# Helpers.css

## Intro

**Helpers.css** is another [eTobb.com](http://www.eTobb.com) Open Source contribution that helps developers build LTR websites that can be easily converted to RTL (and vice versa).
**Helpers.css** also gives you control over responsivity.


## Source

The main file is [helpers.css](https://github.com/JadJoubran/helpers.css/blob/master/src/helpers.css)

## On directions (LTR/RTL)

**Helpers.css** provides classes for margins, paddings, floats, text-aligns and others..
Use those classes instead of writing the rules in your css and your website will be easily convertable to the other direction, by including th rtl.helpers.css which overrides those helpers to behave in the opposite way: .pull-left would float: right, ml5 (margin-left: 5) would do a margin-right: 5, etc..

## On responsivity

**Helpers.css** provides classes for fonts and line-heights.
By using those classes you can extend the helpers.css with your own media queries to change the values of each class. Example [here](https://github.com/JadJoubran/helpers.css/blob/master/examples/example.responsive.css)


## Conventions

**Helpers.css** borrows the same convention from Twitter Bootstrap: .pull-left for float: left, etc..


## Contributors

Developed by Jad Joubran [@JoubranJad](https://twitter.com/joubranjad)