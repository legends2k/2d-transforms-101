# 2D Transforms 101
A presentation/tutorial on 2D transforms for programmers and practitioners favouring intuition over mathematical rigour; animations are used to illustrate the effect of every transform explained. [View it directly in your browser!](http://legends2k.github.io/2d-transforms-101/#/) Press `?` while in the presentation for controls and `Esc` for an overview and quick navigation. Comments and suggestions are [welcome](mailto:legends2k@yahoo.com).

Transformations are a general mathematical concept that is applicable to anyone working in:

* Computer Graphics
    + Animation
    + Game Programming (2D and 3D)
    + Image Processing
    + Motion Capture
    + UI Design
* Computer Vision
* Robotics
* Aeronautics
* Parallel Computing

Concepts discussed are dimension-indepedant; it's just easier to explain and visualize things in 2D but they're applicable to higher dimensions without loss of generality.

Instead of dealing with only elementary transforms (rotate, scale, translate) on points, which most resources do, it also covers:

* Basic math behind transforms (without matrices)
    + Matrices, introduced past the basics since they're just tools
* Composite transforms — concatenation of multiple transforms
    + Anti-commutativity
    + Transforms about an arbitrary origin
* Active and passive viewpoints of transforms
* Transformation of coordinate systems
* Mapping between multiple coordinate systems
* Hierarchical Transforms

## Requirements
The presentation was hand-crafted using HTML5, CSS3, JavaScript and SVG; so nothing more than a browser is required to view the presentation. [Firefox](http://www.firefox.com/), [Chrome](http://www.google.com/chrome/index.html) or [Opera](http://www.opera.com/), even if you've an older version, is highly recommended since support for SVG animations isn't that great in other browsers; with browsers like Safari, Edge or IE you will not be able to see these animations — [caveat lector](http://en.wiktionary.org/wiki/caveat_lector).

You can also view the presentation on a mobile or a tablet; the content, without any loss of fidelity, should get resized and fit to given form factor, thanks to [vector graphics](http://en.wikipedia.org/wiki/Vector_image_format) and CSS3. Touch (tap and swipe left/right) is supported both for navigation and animation control.

## Animations
Transformations are better understood visually than with just dry theory. Hence every transformation workout is accompanied, along with the math, by an animation. Images with a graph sheet background contain animations. Simply click on such an image to cycle through the animation. Every click changes the image's state, animating it into a new figure. When you see the original figure you started with, it denotes the end of all the animation the image contains.

If you're using a keyboard to navigate the presentation, clicking the image steals focus from the presentation and sets in on to the image; simply click anywhere outside the image to give the focus back to the presentation. Now press `space`/`→` to continue with the presentation.

## Solution
The solution to problem of mapping the boy space to street space that is posed at the end of the presentation is in [`map_boy_to_street.md`](https://github.com/legends2k/2d-transforms-101/blob/master/map_boy_to_street.md).

## SVG
The demonstrations/interactive animations embedded within the presentation was done in [SVG](http://en.wikipedia.org/wiki/Scalable_Vector_Graphics), the XML-based, open standard file format for vector graphics with support for animation. In English, all it has are just instructions like `move to`, `line to`, `rect`, `circle`, `ellipse`, etc. in a very readable, XML format and no unintelligible binary data. So a reader (yes, a human one too) can easily read and understand it; a renderer can render it at any resolution without any loss in fidelity. The presentation's first slide has a [3D-transformed background](http://rawgit.com/legends2k/2d-transforms-101/gh-pages/images/2D_affine_xforms.svg) which too is an SVG — it should show up as something similar to [this](http://rawgit.com/legends2k/2d-transforms-101/gh-pages/images/background.png); a simple check to see how well your browser supports SVGs and CSS3 transforms.

It's highly recommended that you fiddle with the SVGs under [`images`](https://github.com/legends2k/2d-transforms-101/tree/gh-pages/images) directory. SVG format is very similar to [PostScript](http://en.wikipedia.org/wiki/PostScript) (which also has commands like `move to`, `line to`, etc.) and is an excellent `Hello World` test bed ([Short, Self Contained, Correct, Example](http://www.sscce.org/)) for learning transformations or 2D graphics in general. Oh they also have a tag for groupings `<g>` which may be used to learn hierarchical transformations. An SVG is only more readable than a PS, PDF or [XAML](http://msdn.microsoft.com/en-us/library/windows/apps/dn535793.aspx). Just open it in a (modern) browser to view it (no, not Edge, it doesn't do 3D CSS3 transforms in SVGs yet :), open it in your favourite text editor, muck around, save and refresh your browser to see the changes immediately; rinse and repeat.

## Credits
* [Computer Graphics using OpenGL](http://amzn.com/0131496700), _Francis Hill_ and _Stephen Kelley_
* [3-D Computer Graphics](http://amzn.com/0521821037), _Samuel R. Buss_
* [Essential Math for Games and Interactive Applications](http://amzn.com/0123742978), _James Van Verth_ and _Lars Bishop_
* [3D Math Primer](http://amzn.com/1568817231), _Fletcher Dunn_ and _Ian Parberry_
* [reveal.js](http://github.com/hakimel/reveal.js), the presentation framework, generously shared under the MIT licence by _Hakim El Hattab_
* [MathJax](http://www.mathjax.org/) for rendering beautiful math equations on any browser, _American Mathematical Society_
* [Elementary affine transforms chart](http://en.wikipedia.org/wiki/File:2D_affine_transformation_matrix.svg) shared under CC 3.0, used as first slide background, _CM Lee_
* [What is or isn't a linear transform](http://commons.wikimedia.org/wiki/File:LinearTransformations.svg), shared under CC 3.0, _Ldo_
* [Reveal.js on Github pages](http://vaskoz.wordpress.com/2013/12/15/reveal-js-on-github-pages/), _Vasko Zdravevski_
