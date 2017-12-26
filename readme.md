# Ionicons For Wildfire

This project is created for building icons for [Wildfire](https://wildfire.js.org). Please visit [ionicons.com](http://ionicons.com) for more about icon-building.

## Build Instructions

This repo already comes with all the files built and ready to go, but can also build the fonts from the source. Requires Python, FontForge and Sass:

1) Install FontForge, which is the program that creates the font files from the SVG files:

    $ brew install fontforge ttfautohint

2) Install [Sass](http://sass-lang.com/)

    $ gem install sass

3) Add or subtract files from the `src/` folder you'd like to be apart of the font files. `src0/` folder contains all the origin files from ionicons, while `src/` contains all the icon files used by `Wildfire`.

4) Run the build command:

    python ./builder/generate.py

5) Copy all file in `./less/` to overwrite files in `iview/src/styles/common/iconfont/`.

6) Copy folder `./fonts` to overwrite folder `iview/src/styles/common/iconfont/fonts`.

Now, all the icons can be used by `iview` for `Wildfire`.

## License

Ionicons is licensed under the [MIT license](http://opensource.org/licenses/MIT).
