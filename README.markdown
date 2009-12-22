Simple Sidebars
===============

Copyright (c) 2009, Colin Gourlay
Email: colin.j.gourlay@gmail.com

Simple Sidebars is a set of css classes that can be used to build fluid-width pages with fixed-width sidebars. Here's a quick example:

    <div class="r300">
        <div class="m">
            <p>Main content goes here</p>
        </div>
        <div class="s">
            <p>Sidebar content goes here</p>
        </div>
    </div>

In the code above, we have a div element with a class "r300". This indicates that this element will contain a fluid-width 'main' content area (denoted by the class 'm'), followed by a 300px fixed-width 'sidebar' (denoted by the class 's'). Different sidebar positionings and widths can be achieved by altering the container's class. The layouts that are currently possible are:

* l180 = 180px sidebar at the left of the page
* l240 = 240px sidebar at the left of the page
* l300 = 300px sidebar at the left of the page
* r180 = 180px sidebar at the right of the page
* r240 = 240px sidebar at the right of the page
* r300 = 300px sidebar at the right of the page

The contents of the container must always be in the order main>sidebar, for the layout to flow correctly. For example, a page with a 240px left sidebar would be marked up as:

    <div class="l240">
        <div class="m">
            <p>Main content comes first</p>
        </div>
        <div class="s">
            <p>Sidebar is still placed second</p>
        </div>
    </div>

This also makes the page more accessible as the main content will always come first in the flow of the document.

I originally designed Simple Sidebars to be used with my fluid-width css framework: class="y" (an example of which is in the demo page), and I recommmend using both together to rapidly build your page layouts. class="y" can be found on GitHub at [http://github.com/colingourlay/classycss](http://github.com/colingourlay/classycss).

Anyone wishing to contribute can email me at: colin.j.gourlay@gmail.com.

I hope you find Simple Sidebars useful.