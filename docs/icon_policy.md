# Icon policy
This document provides guidelines for contributing icons used in the Bitcoin Core software.



## Icon Style
Icon style should follow a few basic principles to maintain consistency and clarity:

- Icons should be minimal with little to no fine details. 
- Icon shapes should be consistent and avoid organic elements that do not scale well.
- Icons should should fit within the 'live area' of the icon grid - see below. 



## Icon Grid
Bitcoin Core's icon set uses an 8-point grid system which utilises size increments of 8 (in pixels) to visually orientate elements within a grid. An even
number like 8 to position icon elements makes scaling on a wide variety of devices easy and consistent. Most popular screen sizes are divisible by 8 which makes 
fitting elements easier with an 8-point grid system. Overall, this makes things more efficient for designers and maintains consistency across applications. 



## Preparing Contribution
When contributing an icon to Bitcoin Core both a source file, in Scalable Vector Graphics (SVG) format, and an optimised production file, in Portable Network 
Graphics (PNG) format, are to be included of said icon.

SVGs are used as source files due to being able to scale to any size whilst retaining image quality but are not used in production due to limited support by 
applications. If different sized production (PNG) icons are required they can be generated from the associated scaled SVG file in a vector based tool like 
Inkspace, Adobe illustrator, Figma, Sketch or Adobe XD.

PNGs are used in production due to their wide support in applications, support of transparent backgrounds and better image quality than competing file types 
such as JPEG.

### Source files (SVG)
Source SVG files should be added to `src/qt/res/src` at 24 x 24px.

### Production files (PNG)
Production PNG files should be added to `src/qt/res/icons` at 24 x 24px.

**Optimizing PNGs:** All production PNG files are to be optmized before being added to Bitcoin Core. Optimizing PNG files removes various color profiles, 
ancillary (alla) and text chunks resulting in a reduction in size of the image file losslessly (without a lowered image quality). Various PNG optimizers exist, 
below are some examples:

- Open source tool [ImageOptim](https://imageoptim.com/api).
- Open source tool [Trimage](https://trimage.org/).
- (Advanced) Run them through Bitcoin Cores [optimize-png.py](https://github.com/bitcoin-core/bitcoin-maintainer-tools/blob/master/optimise-pngs.py) script.



## Attribution 
Icon additions should have the appropriate attribution to the author, the licence used for the icon and any comments relevant to the icon included in the 
[contrib/debian/copyright](https://github.com/bitcoin-core/gui/blob/master/contrib/debian/copyright) file.
