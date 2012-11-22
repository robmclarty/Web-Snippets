# Web Snippets

This is a collection of HTML, CSS, and Javascript pieces that I've found useful in 
various projects. These aren't plugins, but collections of code that work together,
simplified down to their basic elements for each individual function.

This repository will grow over time to include tricks and behaviours I've found
that I would like to re-use in other projects.

If you have any questions, please let me know! I'm happy to help, and take 
help from others :)

R

## What's in here?

### Scrollable Modal Window

![Scrollable Modal Window Screenshot](http://robmclarty.com/screenshots/modal-scrollable.png)

Uses jQuery, CSS, HTML5, and Mustache templates to load a modal window ontop of the base
HTML content using data passed in from JSON. This is meant to emulate the functionality
of Pinterest's modal windows such that the base HTML content can scroll, but then freeze
while the modal window scrolls on top of it (i.e., the scroll-wheel of the mouse starts
working for the modal content rather than continuing to work on the base content).

### Static Modal Window

![Static Modal Window Screenshot](http://robmclarty.com/screenshots/modal-static.png)

Much like the scrollable modal window, only for small messages that don't require
scrolling. Because no scrolling is needed, we can do other fancy things like blur out
the background (blurring has a big performance hit when scrolling ontop of it). This
could be used for flash messages in your Javascript app. 

These two modal window
solutions are very simplified but could easily be adapted to be included in a more
sophisticated setup like Backbone or something. I've not used a bigger framework
here in order to focus solely on the modal functionality itself.

### Fullscreen Background Image Resize + Center

![Fullscreen Background Image Resize + Center Screenshot](http://robmclarty.com/screenshots/fullscreen-background-resize.png)

Apply a full-viewport background image that resizes and centers itself to optimally
cover the viewport with the image while layering a separate content container ontop
using jQuery on the `$(window).resize()` event.

### Mobile Menu

![Mobile Menu Screenshot](http://robmclarty.com/screenshots/mobile-menu.png)

A possible "hidden" menu system for use in mobile web contexts built with 
jQuery + CSS3 transitions. Imagine one of those 3-lined-icons for toggling a menu
off and on so you can save valuable real estate in a constrained mobile view. I've
used "overflow-x: hidden" on the body to prevent horizontal scrolling when the content
gets shoved over while maintaining the main scrollbar to use for moving the content
up and down, however this doesn't allow for scrolling in the menu area which may be
an issue if the menu gets vertically taller than the viewport.

### Double Mobile Menu

![Double Mobile Menu Screenshot](http://robmclarty.com/screenshots/mobile-menu-double.png)

An improvement over the original mobile menu template in that it incorporates some
simple icons to click on in the main, fixed menu and an overlay link which dims the 
main content so that you can click anywhere on the main content area to get back to it. 
This one also includes a hidden menu on either side of the main content in case you 
need extra functionality there.
