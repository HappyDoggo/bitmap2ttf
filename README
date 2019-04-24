Bitmap2ttf converts (monochrome) bitmap fonts into ttf fonts.

There are three parts:

1. **outliner.py:** Traces each bitmap into a series of polygons.

2. **convert.py:** makes the polygons into svg files, and writes a script for FontForge to convert the svgs into a ttf font.

3. **loader of your choice/implementation:**
    - *pcftotty.py:* loader for PCF bitmap fonts.

    Usage: `./pcftottf.py font.pcf`

    - *amigatottf.py:* loader for amiga diskfonts (eg topaz).

    Usage: `./amigatottf.py topaz/11`

    Amiga diskfonts are multiple files in a directory.
    The output will be named after the directory.

The program is structured to make it easy to implement a loader for a font
format of your choice. All you need is to supply a dict object to convert.py
which contains the `key=>value` pairs: `character unicode value => Image`

# Running the Scripts
Dependencies required are Pillow, or PIL and FontForge. Pillow is recommended over PIL as PIL hasn't been maintained in years.

On Mac and Linux, it should be pretty straightforward. However on Windows, to save yourself a lot of trouble, run Linux within a virtual machine or the [WSL.](https://github.com/michaeltreat/Windows-Subsystem-For-Linux-Setup-Guide)

