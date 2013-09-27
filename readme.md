Vanilla HTML
============

Vanilla HTML is a framework built on the concept of not requiring extra markup or class attributes to attain a layout. Just write semantic HTML with some basic knowledge of Vanilla HTML and your layout is done. Seriously, now focus on the things that are actually important, like your design. Oh yeah and Vanilla HTML is 100% responsive.

Demo
----

[Demo](http://tylerchilds.com/projects/vanilla)

Getting Started
---------------

1. Download [vanilla.css](https://raw.github.com/tylerchilds/Vanilla-HTML/master/css/vanilla.css)
2. Add `<link rel="stylesheet" href="vanilla.css">` to your html
3. Toss `class="vanilla"` on an element. I recommend `<body class="vanilla">`

### Templates

<pre>

`<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="initial-scale=1">
        <link rel="stylesheet" href="css/vanilla.css">
    </head>
    <body class="vanilla">
        <header>
            <h1>Page Title</h1>
        </header>
        <hr />
        <section>
            <article>
                Larger Left Column
            </article>
            <aside>
                Smaller Right Column
            </aside>
        </section>
        <hr />
        <footer>
            <section>
                &copy; 2013, Tyler Childs
            </section>
        </footer>
    </body>
</html>`

</pre>

[Download this basic Template](https://raw.github.com/tylerchilds/Vanilla-HTML/master/template.html)

[Documentation] What you need to know
---------------------

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

If these are not good enough and you want a polyfill, you should be able to use [flexie](https://github.com/doctyper/flexie). In case you're wondering, I implemented the old spec and the new spec of flexbox (formerly box) so this polyfill should still work. I chose not to implement the polyfill because this is a framework built for the future.

For more detailed information on the browser support of flexbox: [caniuse.com/flexbox](http://caniuse.com/flexbox)