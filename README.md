#2D-transforms-101
A presentation/tutorial on 2D affine transforms for the programmers and practitioners that tries to develop intuition and goes light on the mathematical rigour. View it [here](http://legends2k.github.io/2D-transforms-101/#/). Comments and suggestions are welcome.

##Requirements
The presentation was hand-crafted using HTML5, CSS3, JavaScript and SVG; so nothing more than a browser is required to view the presentation. However, [Firefox](http://www.firefox.com/) (even if you've an older version) is highly recommended since support for SVG animations with shortcut keys aren't available in any other browser (yes, including Chrome, which is _almost_ there) as yet (14 May, 2015); so in other browsers you mightn't be able to see the interactive animations that well. You may press `?` while in the presentation to get a list of the shortcuts to navigate the presentation.

You can also view the presentation on a mobile or a tablet, as the content only employs [vector graphics](http://en.wikipedia.org/wiki/Vector_image_format), CSS3 is used in a way that it should resize itself without loss of fidelity, to fit a given form factor; it also supports touch events. However, I personally test the presentation only on a Desktop — [caveat lector](http://en.wiktionary.org/wiki/caveat_lector).

##SVG
The demonstrations/interactive animations embedded within the presentation was done in [SVG](http://en.wikipedia.org/wiki/Scalable_Vector_Graphics), the XML-based, open standard file format for vector graphics. In English, all it has is just instructions like `move to`, `line to`, `rect`, `circle`, `ellipse`, etc. in a very readable, XML format and no unintelligible binary data. So a reader (yes, a human too) can easily read and understand it; a renderer can render it at any resolution without any loss in fidelity. The presentation's first slide has a 3D-transformed background which is also an SVG ([this one](https://rawgit.com/legends2k/2D-transforms-101/gh-pages/images/2D_affine_xforms.svg) – click to see how well your browser renders SVGs).

It's highly recommended that you fiddle around with the SVGs under [`images`](https://github.com/legends2k/2D-transforms-101/tree/gh-pages/images) directory. SVG format is very similar to [PostScript](http://en.wikipedia.org/wiki/PostScript) (which also has commands like `move to`, `line to`, etc.) and is an excellent `Hello World` test bed ([Short, Self Contained, Correct, Example](http://www.sscce.org/)) for learning transformations or 2D graphics in general. Oh they also have a tag for groupings `<g>`, like PDF has `XOjbects`; an SVG is only more readable than a PS and PDF. Just open it in a (modern) browser to view it (no, not Edge, it doesn't do 3D CSS3 transforms in SVGs yet :), open it in your favourite text editor, muck around, save and refresh your browser to see the changes immediately; rinse and repeat.

###Animation Shortcuts
To run any animation in the presentation, simply click on it (for it to get the keyboard focus) and press 1, 2, 3, etc. (depending on the number of transforms present it has) and you'd see the animation; to get back to the original state, press `r`. Click elsewhere and press `space`/`→` to continue with the presentation. Alternatively, you may directly open the animation file (`<some_file>.svg` under the `images` directory) in a separate tab and play with the animation there.

##Math Equations
The presentation is math-heavy and some component in a formula may not get rendered, rarely. So if you see some component missing or is illegible, do a `Ctrl` + `F5` to reload the page and the missing component should reappear. Since this is HTML you can skip to any slide directly by just adjusting the slide number in the address bar.

###Solution
The solution to boy space to street space problem is in [`map_boy_to_street.md`](https://github.com/legends2k/2D-transforms-101/blob/master/map_boy_to_street.md).

##Credits
* [Computer Graphics using OpenGL](http://amzn.com/0131496700), _Francis Hill_ and _Stephen Kelley_
* [3-D Computer Graphics](http://amzn.com/0521821037), _Samuel R. Buss_
* [Essential Math for Games and Interactive Applications](http://amzn.com/0123742978), _James Van Verth_ and _Lars Bishop_
* [3D Math Primer](http://amzn.com/1568817231), _Fletcher Dunn_ and _Ian Parberry_
* [reveal.js](http://github.com/hakimel/reveal.js), the presentation framework, generously shared under the MIT licence by _Hakim El Hattab_
* [MathJax](http://www.mathjax.org/) for rendering beautiful math equations on any browser, including ones not supporting [MathML](http://en.wikipedia.org/wiki/MathML) like IE and Edge, _American Mathematical Society_
* [Elementary affine transforms chart](http://en.wikipedia.org/wiki/File:2D_affine_transformation_matrix.svg) shared under CC 3.0, used as first slide background, _CM Lee_
* [What is or isn't a linear transform](http://commons.wikimedia.org/wiki/File:LinearTransformations.svg), shared under CC 3.0, _Ldo_
* [Reveal.js on Github pages](http://vaskoz.wordpress.com/2013/12/15/reveal-js-on-github-pages/), Vasko Zdravevski
