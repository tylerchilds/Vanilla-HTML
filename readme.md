Vanilla HTML
============

Vanilla HTML is a framework built on the concept of not requiring extra markup or class attributes to attain a layout. Just write semantic HTML with some basic knowledge of Vanilla HTML and your layout is done. Seriously, now focus on the things that are actually important, like your design. Oh yeah and Vanilla HTML is 100% responsive.

**[View Demo](http://tylerchilds.com/projects/vanilla-html/demo.html)**

Getting Started
---------------

1. Download [vanilla.css](https://raw.github.com/tylerchilds/Vanilla-HTML/master/css/vanilla.css)
2. Add `<link rel="stylesheet" href="vanilla.css">` to your html
3. Toss `class="vanilla"` on an element. I recommend `<body class="vanilla">`

### Templates

**[Download this basic Template](https://raw.github.com/tylerchilds/Vanilla-HTML/master/template.html)**

<pre>

&lt;!DOCTYPE html&gt;
&lt;html&gt;
    &lt;head&gt;
        &lt;meta name="viewport" content="initial-scale=1"&gt;
        &lt;link rel="stylesheet" href="css/vanilla.css"&gt;
    &lt;/head&gt;
    &lt;body class="vanilla"&gt;
        &lt;header&gt;
            &lt;h1&gt;Page Title&lt;/h1&gt;
        &lt;/header&gt;
        &lt;hr /&gt;
        &lt;section&gt;
            &lt;article&gt;
                Larger Left Column
            &lt;/article&gt;
            &lt;aside&gt;
                Smaller Right Column
            &lt;/aside&gt;
        &lt;/section&gt;
        &lt;hr /&gt;
        &lt;footer&gt;
            &lt;section&gt;
                &copy; 2013, Tyler Childs
            &lt;/section&gt;
        &lt;/footer&gt;
    &lt;/body&gt;
&lt;/html&gt;

</pre>

**[Download this basic Template](https://raw.github.com/tylerchilds/Vanilla-HTML/master/template.html)**

### Use Vanilla with existing HTML

Want to use Vanilla somewhere in your existing code? Include [vanilla-extract.css](https://raw.github.com/tylerchilds/Vanilla-HTML/master/css/vanilla-extract.css)

Then add class="vanilla" to an element and the descendants will behave accordingly.

[Documentation]
---------------

### What you need to know

**GRID:** Start a grid by adding class="vanilla" to an element. This is the only CSS class in the API. For a simple layout all you need is &lt;body class="vanilla"&gt;

**ROWS:** Elements that are direct children of class="vanilla" will become ROWS.

**COLUMNS:** Direct children of ROWS will be COLUMNS. Columns are weighted depending on the tag. header, section, nav, article, main, address, and footer tags produce a larger column when placed next to any other tag. Using this technique you can create an assortment of different column layouts. 

**Note:** To achieve optimal responsive media, do not place media elements (img, video, iframe) as direct children of rows. 
**Tables:** It's a great idea to not use tables for grids, rows or columns, so great, in fact, NEVER do it. Just nest your tables inside a column and they'll play nice.

Seriously, that's all there is to it. You can nest a GRID anywhere to achieve extra nestings.

Browser Support
---------------

Flexbox stuff is still pretty new, so older browsers don't support it. Below are the browsers that support the techniques I'm using.

+ IE 10+
+ Firefox 2+
+ Chrome 4+
+ Safari 3.1+
+ Opera 12.1+
+ iOS 3.2+

For IE 7, 8 and 9, the layout collapses to 1 column. It works about 90% to my liking in those browsers, but considering it's IE, I'm 100% okay with it.

If these are not good enough and you want a polyfill, you should be able to use [flexie](https://github.com/doctyper/flexie). In case you're wondering, I implemented the old spec and the new spec of flexbox (formerly: box) so this polyfill should still work. I chose not to implement the polyfill because this is a framework built for the future.

For more detailed information on the browser support of flexbox: [caniuse.com/flexbox](http://caniuse.com/flexbox)

Credits & Attribution
---------------------

Here are a few tools I used to help bring this together better and faster than on my own.

+ [HTML5 Boilerplate](http://html5boilerplate.com/)
+ [CodeKit](http://incident57.com/codekit/)
+ [Less](http://lesscss.org/)
+ [Less Elements](http://lesselements.com/)
+ [Normalize](http://git.io/normalize)











