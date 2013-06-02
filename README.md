MyStrap
=======

## About


## Why did I write this?
Twitter Bootstrap is the unofficial king of CSS frameworks. So why would I, one kid with very little experience, presume that I could improve on the definitive solution? Honestly, this started out as a little project to fix a few things that I don't like:

1. **Validation**. Bootstrap is littered with hacks, mostly for IE&lte;8, and it doesn't validate. Because of how buggy that browser is, it remains a thorn in every designer's side. Yes, validation is not the goal&ndash;proper display is. But like so many others, it gives me a warm, fuzzy feeling to get that green bar from the validator. MyStrap compiles the same LESS docs twice, once with the IE hacks, and once without, meaning all that's required is an IE conditional to decide which to call.
2. **Semantics**. HTML is supposed to be a semantic language, and HTML5 gives us plenty of beautifully semantic block-level and inline tags. For every `div` I inserted into a site that had no function other than to get my styles to work, I died a little inside. I think the epitome of this is seen in the Bootstrap navbar, especially if you want a collapsible one.
3. **Aesthetics**. I'm not an artist, so anytime I find an aesthetic design concept based out of logic, it makes things easier for me. "Vertical rhythm" is one of those concepts, and Bootstrap didn't have it. MyStrap does.
4. **Design Ease**. I wanted to be able to control nearly every aspect of my base design in a single LESS file. That file was already set up in `variables.less`, I just wanted to expand it so that I could make it do more.
5. **Integration**. I design mostly for Wordpress. It's a simple admin area, and my customers are simple people. I wanted to go back in and rewrite the styles in the framework to fit to Wordpress. The software already injects tons of classes into the markup, so why not use them? Also, I feel it would be worthwhile to integrate all the great features that H5BP, Modernizr, and so many other wonderful open-source projects have made available to us.
6. <small>**Boredom**. I needed a good project.</small>

*NB: I used IE conditionals because it amounts to a smaller file size not having to redeclare styles if hacks are just ported to a separate file, and because the additional HTTP request would further increase load time.*