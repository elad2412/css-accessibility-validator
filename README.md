# Accessibility CSS Validator

**Accessibility CSS Validator, is a tool for finding HTML accessibility errors and warnings on web pages via advanced capabilities of CSS selectors.**

Check out this **[demo][demo]** to see it in action!

## Setup

Very easy, just download this CSS accessibility.css file, and add it to your own project, and you finish.
Refresh your page, and now you can see all the issues that the CSS Accessibility Validator finds.

##What Validation the CSS Accessibility Validator Returns?
The tool checks three levels of Validation: Errors, Warnings and Recommended.

notice: the tool check only stuff we can catch via CSS only.

##The Validation Levels
###Error Level - This is the most critical level of accessibility.
######At this level we can found:
1. Alternative texts for images
2. Empty Tags Links, without ID or a title attribute
3. Empty Headers, or empty headers without a title attribute

The Error will color in red outline.

###Warning Level - At this level are things which may have accessibility errors.
######At this level we can found:
1. Input text fields without placeholder or without sibling label tag(before) with the attribute "for" on it.

The Warning will color in orange outline.

###Recommended Level - This is the less critical level of accessibility.
######At this level we can found un-recommended HTML tags as: iframe , flash tags(embed or object)
1. Flash HTML isn't accessibility.
2. Iframes are half accessibility, if there is a form inside them for example, you can go in but you can't get out of them.
3. Inline Styles - can make issues to screen readers.

The Recommended will color in blue outline.

##Examples
[You can see Live Example in our site]

#####Image Tag Missing Alt
```html
	<img src="http://farm8.staticflickr.com/7443/9733944130_bba200844f_m.jpg">
```

#####Image With Empty Alt or Title Attribute
```html
	<img src="http://farm8.staticflickr.com/7443/9733944130_bba200844f_m.jpg" alt="">
```

#####Empty Link Tag - with no anchor(ID) or no title attribute or no inner text
```html
	<a href="http://elad2412.github.io/css-accessibility-validator/"></a>
```

###Header with no text or title attribute
```html
	<h3 class="something"></h3>
```

#####Check Validation of input with no-placeholder or element "label" before
```html
	<input type="text">
```

#####Flash Tag aren't accessibility
```html
	<embed width="100" height="50"></embed>
	<object width="100" height="50"></object>
```

#####Ifames are half accessibility, if there is a form inside them for example, you can go in but you can't get out of them.
```html
	<iframe width="100" height="50"></iframe>
```

#####Inline Styles - can make issues to screen readers.
```html
	<div style="color:purple; font-weight:bold;">this element has Inline Styles</div>
```


## Browser Support
1. All Browser
2. Internet Explorer from version 10

## Author
**Elad Shechter**, You can find me in this social groups.
[coderwall], [codepen], [twitter], [instagram]
+ [![endorse](https://api.coderwall.com/elad2412/endorsecount.png)](https://coderwall.com/elad2412)

**Forum Groups:**

**International Facebook Group**: [css-masters-group]

**Israeli Facebook Group**: [css-masters-israel-group]

## License

Licensed under [MIT][mit]. Enjoy.

[demo]: http://elad2412.github.io/css-accessibility-validator/#examples
[You can see Live Example in our site]: http://elad2412.github.io/css-accessibility-validator/#examples
[coderwall]: https://coderwall.com/elad2412
[codepen]: http://codepen.io/elad2412/
[css-masters-group]: https://www.facebook.com/groups/css.master/
[css-masters-israel-group]: https://www.facebook.com/groups/css.masters.israel/
[twitter]: https://twitter.com/eladsc
[instagram]: http://instagram.com/elad_2412
[mit]: http://www.opensource.org/licenses/mit-license.php

