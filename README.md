iview
=====
A quick and simple image viewer for Linux, based on Python and Qt

Requirements
============
Running iview requires Qt and PyQt installed. iview program is a
single python file.

Usage
=====
Calling iview requires specifying one or more image file names.
When a single file is specified the list of all files with a known
extension in the same directory is used as image list for prev/next.

Key bindings
============
- Left arrow : previous file
- Right arrow : next file
- "R" : Rotate image
- "C" : Crop image
- "S" : Save image as
- "1", "2", "3", "4" : Sets exact 1/1, 2/1, 3/1 or 4/1 pixel scaling
- "0", Home : Zoom image to fit view
- "F" : Fullscreen on/off

Mouse drag does panning, mouse wheel does zooming.

Features
========
- Smooth scaling when zooming out, hard scaling when zooming in
- When changing to next/prev picture the view is not changed if
  picture size is the same (allows looking at several images as
  an animation)
- Updating the image on disk updates the view (live display)
- Zoom is centered on mouse position
- Transparency support
- Rotation, cropping and format conversion with "save as..."
- Supports most image formats (anything QImage accepts).
  On my system the list of known extensions is:
  bmp, bw, bw, dds, eps, eps, epsf, epsf, epsi, epsi, exr, exr,
  gif, ico, jp2, jpeg, jpg, mng, pbm, pcx, pcx, pgm, pic, png,
  ppm, psd, psd, ras, ras, rgb, rgb, rgba, rgba, sgi, sgi, svg,
  svgz, tga, tga, tif, tiff, xbm, xcf, xcf, xpm, xv.
