# Handy: A mobile first grid boilerplate thingummy

*Major Caveat: This is my personal method for a small number of sites. It has a number of requirements if you don't want it to break in IE6*

Requirements:

* Respond.js or css3-mediaqueries.js
* Selectivizr to polyfill for CSS3 selector compatibility in older browser versions

## What's all this 'Major Caveat' all about?

The important thing to understand is that I design in a specific way that is possibly unique/wrong/stupid/insane. Bearing that in mind, if you like the idea of a basic grid system that prefers mobile first over desktop resolutions, then it's a good start.

But really, possibly unique/wrong/stupid/insane.

# So how do I use it?

The premise is pretty simple but differs in some ways from the accepted norms in grid layouts. You start with a major wrapper element (`<div>` and also `<section><aside><article>`) and give it a class of `fwrap` and additionally the number of columns `c2 c3 c4`.

After this, you just populate your wrapper with subsections equal to the number of columns (`<div><section><aside><article>`), eg:

    <div class="fwrap c4">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
    </div>

You can mix elements and use sections, articles and divs and it will simply work.

If you want one column to span multiples, you can add a class to expand it. f23 means 2 columns out of a 3 column layout, f24 2 columns of a 4 column layout, f34 3 columns of a 4 column layout.

* I haven't finished writing this README yet. Will update soon, I promise x *
