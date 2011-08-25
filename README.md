# Handy: A mobile first grid boilerplate thingummy

*Major Caveat: This is my personal method for a small number of sites. It has a number of requirements if you don't want it to break in IE6*

I'm currently refactoring a lot of things as it is a method that's evolved throughout different designs. I'm hoping to get the opportunity to bring the improvements here so I can fix bugs more efficiently.

Requirements:

* Respond.js or css3-mediaqueries.js
* Selectivizr to polyfill for CSS3 selector compatibility in older browser versions
* The ie6, ie7, ie8 class trick as popularised by HTML5Boilerplate

## What's all this 'Major Caveat' all about?

The important thing to understand is that I design in a specific way that is possibly unique/wrong/stupid/insane. Bearing that in mind, if you like the idea of a basic grid system that prefers mobile first over desktop resolutions, then it's a good start.

But really, possibly unique/wrong/stupid/insane.

Also bear in mind that there are bloody loads of subtle nuances to designing a responsive grid. In my opinion, this is mostly handy for quick prototyping. Once you have a prototype, you will really want to consider how your grid will break down at smaller levels; this is something I don't feel that a boilerplate/framework should do for you.

# So how do I use it?

The premise is pretty simple but differs in some ways from the accepted norms in grid layouts. You start with a major wrapper element (`<div>` and also `<section><aside><article>`) and give it a class of `hwr` and additionally the number of columns `hc2 hc3 hc4`.

After this, you just populate your wrapper with subsections equal to the number of columns (`<div><section><aside><article>`), eg:

    <div class="hwr hc4">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
    </div>

You can mix elements and use sections, articles and divs and it will simply work.

If you want one column to span multiples, you can add a class to expand it. hs2 means it will span 2 columns out of the current N column layout, hs3 means it will span 3 columns of the current N  column layout.

* I haven't finished writing this README yet. Will update soon, I promise x *
