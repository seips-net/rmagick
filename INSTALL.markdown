# Windows

## Working with

* Windows 7 professional 64bit & Ruby 1.9.3-p125
* Windows XP SP3 32bit & Ruby 1.9.3-p125

## Install

1. Install [Ghostscript](http://sourceforge.net/projects/ghostscript/) from [gs905w32.exe](http://downloads.sourceforge.net/project/ghostscript/GPL%20Ghostscript/9.05/gs905w32.exe).
2. Install [ImageMagick](http://www.imagemagick.org) from [ImageMagick-6.7.6-3-Q16-windows-dll.exe](http://www.imagemagick.org/download/binaries/ImageMagick-6.7.6-3-Q16-windows-dll.exe)
   * Install dev headers (Check!)
   * Install into C:\opt (You can use any other place witout spaces in the path.}
3. Restart your console / comand prompt / IDE / ... or just restart windows to make ImageMagick commands available.
4. Install rmagick
   <code>gem install rmagick --platform=ruby -- --with-opt-lib=C:/opt/ImageMagick-6.7.6-Q16/lib --with-opt-include=c:/opt/ImageMagick-6.7.6-Q16/include</code>


## Trouble shooting
* The versions of the downloadable software is changing form time to time. Do not give up, if the link is down. Visite the website and look for the next newer version.
* Spaces in the installation path of ImageMagick cause serious problems.
* If you installed rmagick to a different path change the path in the gem command as well.  