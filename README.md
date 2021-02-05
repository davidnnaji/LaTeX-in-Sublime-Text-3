# LaTeX-in-Sublime-Text-3
A visual guide for makming LaTeX editor in Sublime.

# Background
LaTeX is a beautiful tool for academic writing and there are many editing environments built on the Tex platform that are freely available. My favorite editor is Overleaf but there are features that the platform offers that are blocked by a pay-wall. This is a visual guide for setting up a similar LaTeX editing environment in Sublime Text 3 (ST3) using open-source packages for Windows 10. Build instructions for Mac OS and Linux devices are provided in the official documentation for LaTeXTools.

<img src="LatexinSublimeDemo.gif" alt="Latex in Sublime Demo" style="width: 900px;"/>

## Notable Features
Here are some notable features in the base build for Windows:

- Quick and lightweight document preview
- Reverse search
- Forward search
- Inline image preview
- All your favorite Sublime editing features!

A full list of features offered by LaTeXTools can be found [here](). More capabilities can be added as desired by installing additional packages created by the community. Examples are provided in the 'Additional Resources' section along with descriptions of my own perosnal favorites.

## Minimum Requirements
- Windows 10 (x64)
- Sublime Text 3
- A Tex distribution (i.e. MiKTeX or TexLive)
- Sumatra PDF

# Installation

## Install the Required Software
### Sublime Text 3 (x64)
The latest version of ST3 is available for download [here](https://www.sublimetext.com/).

### MikTeX or TexLive
Both [MiKTeX](https://miktex.org/download) and [TexLive](https://tug.org/texlive/) will work with the LaTeXTools package on Windows. TexLive will take longer to initially install but has all the required Tex packages to get running. MiKTeX appears to be more popular and has a shorter initial installation. However, a couple missing packages will need to be downloaded on the first build. Pick one and follow the relevant documentation.

### Sumatra 
The [Sumatra PDF Viewer](https://www.sumatrapdfreader.org/free-pdf-reader.html) is recommended by the developers of LaTeXTools. Its very lightweight and supports both forward and inverse search. It is also the only viewer supported on Windows that is compatible with LaTeXTools.


## Update system PATH Variable
The system `PATH` variable can be modified in the Command Prompt or through Sytem Properties window in the Control Panel. The simplest way is to get the location of any program search for the program in the Windows search bar, open the file location, and open the file properties. Copy the address in the target field and remove the part of the address that references the `.exe` file. Regardless of the method, ensure the executable file for the following programs are included in your system `PATH`.

<img src="FindLocationExample.gif" alt="Find Executable Location Example" style="width: 900px;"/>

1. Ensure that Sublime Text is in your path
2. Ensure that your selected Tex distribution (MiKTeX or TexLive) is in your path
3. Ensure that SumatraPDF is in your path

Follow the same procedure if you plan on installing [Ghostscript](###Ghostscript) or ImageMagick.

## Install Package Control and the LaTexTools Package
The easist way to install the LaTeXTool package is with [Package Control](https://packagecontrol.io/installation). Package Control makes it easy to install and remove ST3 packages. Once installed, open the command pallete again. Type `Package Constrol: Install Package`, press `enter`, then type `LateXTools`, and press `enter`.

## Configure LaTeXTools Settings
To open the LaTeXTools User settings in Sublime navigate to 

## Setup Sumatra


## Test Build
Change the build system to Latex `Tools > Build System > LaTeX`
Download the example Latex files or create your own
Click `Tools > Build` or `Ctrl+B` to build.
Turn on Spell Check

## Install Optional Software
### Ghostscript
[Ghostscript](https://ghostscript.com/download/gsdnld.html) allows equation previewing in the Sublime editor. If you downloaded MiKTeX or TexLive Ghostscript will already be installed. If you are experiencing troubles confirm that your system `PATH` includes references to the Tex distrubution you selected (MiKTeX or TexLive). If you are still lacking math preview functionality, install the Ghostscript general public release.

### ImageMagick
[ImageMagick](https://imagemagick.org/script/download.php#windows) augments the image preview capabilities that come with LaTeXTools (i.e. anything other than PNGs, JPEGs, GIFs, PDFs, EPSs, and PSs). During installation, ensure that only 'Add applicaiton directory to system path' is selected when prompted. Once ImageMagick is installed, ensure the executable directory location is added to your system `PATH` variable. Restart ST3 and hover over any `\includegraphics{}` commands. If graphics are still not displayed check that **FIX dsign ->** `;PATH` is appended at the end of `"texpath"` in the LaTeXTools Windows platform settings.

<img src="Imagemagick.png" alt="ImageMagick Before and After" style="width: 900px;"/>

## Install Additional Sublime Packages
### LaTeXTab

### Github Workflow

# Additional Resources

# Bonus Tips and Tricks
## Pandas Dateframe to LaTeX Table
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_latex.html

# References 

[1] LaTeX Project Official Website. https://www.latex-project.org/

[2] LaTeXTools Documentation. Available: https://latextools.readthedocs.io/en/latest/ 

[3] LaTeXTools Package Page. Available: https://packagecontrol.io/packages/LaTeXTools

[4] Setup for LaTeX and Sublime Text 3 by Daniel Herber. Available: https://www.danielherber.com/guides.php?option=latex-st3