---
title: 'Animated PNG'
date: 2018-11-28T15:14:39+10:00
weight: 1
---

Draw animated PNG images in web pages.
<!--more-->
<div style="float: right;">
  <script type="text/javascript" src="/animatedpng/animatedpng.js"></script><br />
  <script type="text/javascript">
    fishAnim = new AnimatedPNG('fish', '/animatedpng/fish0001.png', 23, 100);
    fishAnim.draw(false);
  </script>
</div>

PNG images have rightly superseded GIFs for many small images on the web, with
many well-known advantages over the older format. However, one area where PNG
lags behind is its lack of an equivalent for small animations, for which animated
GIFs are still the preferred format. Although efforts are under way to create an
[animated PNG format](http://wiki.mozilla.org/APNG_Specification), it will be
some time before it is widely supported.

In the meantime, AnimatedPNG is a Javascript library that takes a sequence of
individual PNG images and draws them in turn, creating the functional equivalent
of the animated GIF. The library is designed to be as simple to use as possible,
with just two lines of javascript to draw a basic animation, and a few extra functions
for more detailed control of the animation. Further details for using the library can
be found on the example page.

### Requirements

There are no special requirements for using the AnimatedPNG library.
All you need is the library file itself, and a set of suitably named PNG image files.

### Compatibility

The library is compatible with pretty much everything. It was written in the days
of Internet Explorer 6 and it even worked with that.

If you do find an incompatibility, please contact me.

### Installation and Usage

The AnimatedPNG library is supplied as a `.tar.gz` or `.zip` file, and contains
the following files:

| File                   | Purpose                                                                           |
| ---------------------- | ----------------------------------------------------------------------------------|
| `animatedpng.js`       | The javascript library in compressed form – use this in your web page.            |
| `animatedpng_large.js` | The javascript library in verbose form, which is easier to understand and modify. |
| `README.txt`           | A readme file giving an overview of how to use the library.                       |

Full details of the API for the Javascript library can be found on the API Page.
An example page showing the library in action can be found here.

Note: Since this library uses individual image files for its frames, it is suitable only for short, simple animations. Longer animations will work, but it may produce odd results while all the images load.

### Latest Release

The latest version is 1.02 (released 2014-11-03), available for download as follows:

* [animatedpng-1.02.tar.gz](https://github.com/squaregoldfish/AnimatedPNG/archive/v1.02.tar.gz) (16Kb)
* [animatedpng-1.02.zip](https://github.com/squaregoldfish/AnimatedPNG/archive/v1.02.zip) (16Kb)

or you can visit the [GitHub page](https://github.com/squaregoldfish/AnimatedPNG)

See the Changelog for what’s new.
AnimatedPNG is released under the terms of the GNU Public License.