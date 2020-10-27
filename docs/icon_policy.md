# Icon policy
This document provides guidelines for contributing icons used in the Bitcoin Core GUI.



## Preparing Icons
Both an icon source file, in Scalable Vector Graphics (SVG) format, and an optimised production file, in Portable Network Graphics (PNG) format, are required for 
each icon.

SVGs are used as source files due to being able to scale to any size whilst retaining image quality, but are not used in production due to limited support by 
applications. If different sized production (PNG) icons are required they can be generated from the associated scaled SVG source file in a vector based tool like 
Inkspace, Adobe illustrator, Figma, Sketch or Adobe XD.

PNGs are used in production due to their wide support in applications, support of transparent backgrounds and better image quality than competing file types 
such as JPEG.

### Icon Style
Icon style should follow a few basic principles to maintain consistency and clarity:

- Icons should be minimal with little to no fine details. 
- Shapes should be consistent and avoid organic elements that do not scale well.
- Colors should be consistent with other icons used in Bitcoin Core. 
- Icons should should fit within the 'live area' of the icon grid - see below.

### Icon Grid
Bitcoin Core's icon set uses an 8-point grid system which utilises size increments of 8 (in pixels) to visually orientate elements within a grid. An even
number like 8 to position icon elements makes scaling on a wide variety of devices easy and consistent. Majority of screen sizes are divisible by 8 which makes 
fitting elements easier using an 8-point grid system. If icons need to be scaled up or down for whatever reason they should stick within multiples of 8 to maintain visual consistancy.

Overall, this makes things more efficient for designers and maintains consistency across applications. Below is an example of an icon within an 8-point grid system. Icons should remain within the live area shown below to prevent being obscurbed by other elements

![](https://github.com/Bosch-0/Project-Muggle/blob/master/assets/images/Icon_grid.svg)


### Optimizing Production Files (PNG): 
Production (PNG) files are to be optmized before being added to Bitcoin Core. Optimizing PNG files removes various color profiles, ancillary (alla) and text chunks resulting in a reduction in size of the image file losslessly (without a lowered image quality). Any `zopflipng` / `pngcrush` based PNG optimizers can be used, below are some examples:

- Open source tool [ImageOptim](https://imageoptim.com/api).
- Open source tool [Trimage](https://trimage.org/).
- (Advanced) Run them through Bitcoin Cores [optimize-png.py](https://github.com/bitcoin-core/bitcoin-maintainer-tools/blob/master/optimise-pngs.py) script.



## Contributing
Icons should only be added to the Bitcoin Core repo via a pull request (PR) in two situations:

- An icon used in production is being replaced with a new icon.
- A feature is being added to the Bitcoin Core GUI that requires the addition of a new icon.

If a new icon is designed for an upcoming or active PR, the designer of the icon should [open an issue](https://github.com/bitcoin-core/gui/issues/new/choose) to get feedback on the design and to make sure it is consistent with Bitcoin Core's iconography.

If a new feature is being added to the Bitcoin Core GUI that requires a new icon the developer should [open an issue](https://github.com/bitcoin-core/gui/issues/new/choose) requesting an icon to be designed. 

Icons (both SVG and PNG) should not be added to the Bitcoin Core repo if they are not yet used in production.

When opening a PR that adds an icon source (SVG) files should be added to `src/qt/res/src` at 24x24px and otimized production (PNG) files should be added to `src/qt/res/icons` at 24x24px. 

### Icon Sizing
Different sized icons sizes may be necessary in some circumstances. If 24x24 is too small or too large for the required icon placement, then the icon should be scaled up or down whilst sticking to the 8-point grid system. Testing of various icon sizes will be required to find the most optimal size that is both not too small reducing image and not too large resulting in unecessary file sizes.



## Attribution 
Icon additions should have the appropriate attribution to the author, the licence used for the icon and any comments relevant to the icon included in the 
[contrib/debian/copyright](https://github.com/bitcoin-core/gui/blob/master/contrib/debian/copyright) file.
