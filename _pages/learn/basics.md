---
mediawiki: Introduction
title: Introduction
section: Learn:ImageJ Basics
nav-links: true
---

# What is ImageJ?

 <a href="/software/imagej"><img src="/media/icons/imagej.png" height="48px"/></a> [ImageJ](/software/imagej) is an [open source](Open_source) [image processing](/imaging) program for multidimensional image data with a focus on scientific imaging.

# What is Fiji?

<a href="/software/fiji"><img src="/media/icons/fiji.png" height="48px"/></a> [<span style="color: darkcyan; font-size: large; font-weight: bold">F</span>iji <span style="color: darkcyan; font-size: large; font-weight: bold">I</span>s <span style="color: darkcyan; font-size: large; font-weight: bold">J</span>ust <span style="color: darkcyan; font-size: large; font-weight: bold">I</span>mageJ](/software/fiji)—a "batteries-included" distribution of ImageJ which includes many useful [plugins](/plugins) [contributed by the community](/contribute/fiji).

# What does ImageJ provide?

| [Application](/software/imagej#flavors)    | A user interface with functions to load, display, and save images. |
| [Techniques](/imaging)                     | [Image processing](/ij/docs/guide/146-29.html#toc-Section-29), [colocalization](/imaging/colocalization-analysis), [deconvolution](/imaging/deconvolution), [registration](/imaging/registration), [segmentation](/imaging/segmentation), [tracking](/imaging/tracking), [visualization](/imaging/visualization) and much more. |
| [Plugins](/plugins)                        | A powerful mechanism for extending ImageJ in all kinds of useful ways. |
| [Scripting](/scripting)                    | Automated, reproducible workflows via [scripts](/scripting) and [macros](/scripting/macro), including [headless on a remote server or cluster](/scripting/headless). |
| [Forum](https://forum.image.sc/tag/imagej) | A vibrant, diverse, and helpful user [community](/discuss) that gives rise to insightful scientific exchanges. |

ImageJ's [extensibility](/develop/architecture#extensibility) is the root of its effectiveness: many advanced image-processing methods are not provided by the core application, but rather are [plugins](/plugins) written by specialists in specific fields, made available via [update sites](/update-sites).

# How do I get started?

## Installation

First, you should to [download](/downloads) and install ImageJ!

## The main window

After starting ImageJ, you will see the main window:

![](/media/learn/fiji-main-window.jpg)

On macOS, the menu bar will appear on the top of the screen (as with all macOS applications).

### The search bar

{% include warning/stub %}

### The menu bar

In the menu bar, you will find most of the functionality, such as loading/saving files, processing them, and plugins will be installed into the menus, too.

The menus have different purposes:

| File    | File input/output, new files      |
| Edit    | Selection/ROI handling            |
| Image   | Visualization, stack manipulation |
| Process | Image filters                     |
| Analyze | Statistics                        |
| Plugins | Plugins, Macros and Utilities     |
| Window  | Windows                           |
| Help    | Help & Links                      |

### The tool bar

The toolbar mostly contains selection tools: the rectangle, ellipse, polygon, freehand and straight line selection tool. By clicking on the icon, you activate the tool.

Some tools offer option dialogs which you can open by double clicking the icon. This example shows the option dialog of the Oval Tool:

![](/media/learn/oval-tool-option-dialog.png)

If there is a small red arrow in the lower right corner of the tool icon, you can right-click ({% include key keys='Ctrl|Left Click' %} on an Apple mouse) and select an alternative selection tool (e.g. a circular brush selection tool which shares the icon with the ellipse selection tool). Example:

![](/media/learn/alternative-tools.png)

### The status bar

The status bar displays useful information at startup, and when running plugins. It also shows a progress bar on the right side for long-running processes:

![](/media/learn/status-bar-with-progress.png)

A single mouse click on the status bar will show the information about ImageJ and Java version as well as about memory consumption:

![](/media/learn/default-status-message.png)

### Drag & Drop

You can drag files from your favorite file manager and drop them on the main
window; ImageJ will load the corresponding files.

Drag 'n Drop will also work for images displayed in your web browser, unless
they are links to other web pages. You can try with images from this page.

## Image windows

Whenever you open an image, be it via {% include bc path='File | Open'%},
Drag 'n Drop or {% include bc path='File | Open Samples'%}, ImageJ will open
an image window.

![](/media/learn/clown-snapshot.jpg)

The window has the file name as title, and it display some useful information
above the image: the real resolution (in this case in square centimeters), the
pixel resolution, the image type and the memory required by the image.

If your image does not have meta-data about the real resolution, you can set
the resolution explicitely with {% include bc path='Image | Properties...'%} or
by following the
[tutorial on spatial calibration](/imaging/spatial-calibration).

### Image Types

You can change the image *type*:

![](/media/image-types.png)

Choose between

-   8-bit (intensity range 0..255)
-   16-bit (intensity range 0..65535)
-   32-bit (floating point numbers)
-   8-bit color (up to 256 colors encoded via a color lookup table)
-   RGB color (3 colors encoded as 8-bit values)

There are two more options: RGB stack and HSV stack, which can turn a 2-dimensional color image into a stack consisting of 3 color channels (red, green & blue or hue, saturation & value, respectively).

## Further reading

Peruse the [user guides](/learn/user-guides),
additional [tutorials](/tutorials), and
[presentations](/events/presentations).
