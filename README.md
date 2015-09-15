#2D Affine Transforms 101
A presentation/tutorial on 2D affine transforms for programmers and practitioners favouring intuition over mathematical rigour. [View it directly in your browser!](http://legends2k.github.io/2d-transforms-101/#/) Press `?` while in the presentation for shortcut keys and `Esc` for an overview and quick navigation. Comments and suggestions are [welcome](mailto:legends2k@yahoo.com).

Instead of dealing with only elementary transforms (rotate, scale, translate) on points, which most resources do, this also shows how to deal with composite transforms (contatenation of multiple transforms) both from active and passive viewpoints. It not only illustrates transformation of points but also transformation of coordinate systems when multiple matrices are involved.

##Requirements
The presentation was hand-crafted using HTML5, CSS3, JavaScript and SVG; so nothing more than a browser is required to view the presentation. However, [Firefox](http://www.firefox.com/) (even if you've an older version) is highly recommended since support for SVG animations with shortcut keys aren't available in any other browser (yes, including Chrome, which is _almost_ there) as yet (14 May, 2015); so in other browsers you mightn't be able to see the interactive animations that well.

You can also view the presentation on a mobile or a tablet, as the content only employs [vector graphics](http://en.wikipedia.org/wiki/Vector_image_format); CSS3 is used in a way that it should resize itself without loss of fidelity, to fit a given form factor; it supports touch events (swipe left/right). However, I personally tested the presentation only on a Desktop — [caveat lector](http://en.wiktionary.org/wiki/caveat_lector).

##SVG
The demonstrations/interactive animations embedded within the presentation was done in [SVG](http://en.wikipedia.org/wiki/Scalable_Vector_Graphics), the XML-based, open standard file format for vector graphics with support for animation. In English, all it has is just instructions like `move to`, `line to`, `rect`, `circle`, `ellipse`, etc. in a very readable, XML format and no unintelligible binary data. So a reader (yes, a human one too) can easily read and understand it; a renderer can render it at any resolution without any loss in fidelity. The presentation's first slide has a [3D-transformed background](http://rawgit.com/legends2k/2d-transforms-101/gh-pages/images/2D_affine_xforms.svg) which too is an SVG — it should show up as something similar to [this](http://rawgit.com/legends2k/2d-transforms-101/gh-pages/images/background.png); a simple check to see how well your browser supports SVGs and CSS3 transforms.

It's highly recommended that you fiddle around with the SVGs under [`images`](https://github.com/legends2k/2d-transforms-101/tree/gh-pages/images) directory. SVG format is very similar to [PostScript](http://en.wikipedia.org/wiki/PostScript) (which also has commands like `move to`, `line to`, etc.) and is an excellent `Hello World` test bed ([Short, Self Contained, Correct, Example](http://www.sscce.org/)) for learning transformations or 2D graphics in general. Oh they also have a tag for groupings `<g>` which may be used to learn hierarchical transformations; an SVG is only more readable than a PS, PDF or [XAML](http://msdn.microsoft.com/en-us/library/windows/apps/dn535793.aspx). Just open it in a (modern) browser to view it (no, not Edge, it doesn't do 3D CSS3 transforms in SVGs yet :), open it in your favourite text editor, muck around, save and refresh your browser to see the changes immediately; rinse and repeat.

###Animation Shortcuts
Images with a graph sheet background contain animations. Simply click on such an image (for it to get the keyboard focus) and press 1 to see the first animation. Then press 2 to see the next, go on till no change happens. The number of animations you see depends on the number of transforms the image contains. To get back to the first frame, press `r`. Click elsewhere and press `space`/`→` to continue with the presentation. Alternatively, you may directly open the animation file (`<some_file>.svg` under the `images` directory) in a separate tab and play with the animation there.

###Solution
The solution to boy space to street space problem is in [`map_boy_to_street.md`](https://github.com/legends2k/2d-transforms-101/blob/master/map_boy_to_street.md).

##Credits
* [Computer Graphics using OpenGL](http://amzn.com/0131496700), _Francis Hill_ and _Stephen Kelley_
* [3-D Computer Graphics](http://amzn.com/0521821037), _Samuel R. Buss_
* [Essential Math for Games and Interactive Applications](http://amzn.com/0123742978), _James Van Verth_ and _Lars Bishop_
* [3D Math Primer](http://amzn.com/1568817231), _Fletcher Dunn_ and _Ian Parberry_
* [reveal.js](http://github.com/hakimel/reveal.js), the presentation framework, generously shared under the MIT licence by _Hakim El Hattab_
* [MathJax](http://www.mathjax.org/) for rendering beautiful math equations on any browser, including ones not supporting [MathML](http://en.wikipedia.org/wiki/MathML) like IE and Edge, _American Mathematical Society_
* [Elementary affine transforms chart](http://en.wikipedia.org/wiki/File:2D_affine_transformation_matrix.svg) shared under CC 3.0, used as first slide background, _CM Lee_
* [What is or isn't a linear transform](http://commons.wikimedia.org/wiki/File:LinearTransformations.svg), shared under CC 3.0, _Ldo_
* [Reveal.js on Github pages](http://vaskoz.wordpress.com/2013/12/15/reveal-js-on-github-pages/), _Vasko Zdravevski_
