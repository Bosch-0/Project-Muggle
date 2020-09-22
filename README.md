# Bitcoin-Core-Design-Foundations [WIP] 

Currently there lacks design foundations within Bitcoin Core making it difficult on-boarding new designers as well as intergrating developers into the design process. This has created a catch-22 situation for contributing designs to Bitcoin Core, as designers are unlikely to create designs if there is no developer to implement them and vice versa for developers implementing designs with limited designer guidance. Establishing some design foundations will help remediate this issue and ultimately result in making software such as the Bitcoin Core GUI more accessible to your average user.

## Goals

The primary overarching goal is to bridge the gap between the Bitcoin Core community and the Bitcoin Design community. 

### General goals:

- Establish a design system for Bitcoin Core to:
  - Assist with on-boarding new designers and developers.
  - Streamline the design and development process and contribution.
  
- Contribute incremental, conservative but impactful UI/UX changes to the Bitcoin Core GUI. This will assist with establishing design implementation flows that work for both developers and designers. 
  
- Be an active design focused PR reviewer for the Bitcoin Core GUI repo.

- Keeping dialogues going between Bitcoin Core developers and designers around design based decisions. [Here](https://github.com/bitcoin-core/gui/issues/89) is an example around the branding of Bitcoin Core. 

- Represent users in many conversations on Github / IRC / Slack that shape the Bitcoin Core GUI. 

- Collaborate with Bitcoin Core design researchers such as Jamaal when it comes to making design decisions. [Jamaal’s Project Horizon.](https://docs.google.com/document/d/1Z2D1Wn5tkQ-Scdp0n8qm2mnFvik1wnU3vcu1DZ1f9jo/edit#)

- Apply what I learn working on designs with Bitcoin Core to the [Bitcoin Design Guide.](https://github.com/BitcoinDesign/Guide)
  - An example being the section on Open Design. I'd imagine insight gained from implementing designs with the Core developers will be useful.

### Specific goals:

- Increase Bitcoin Core node count to ~20k by end of 2021 (currently around ~10k). Bitcoin Core is still the primary Bitcoin node software. By improving the UI/UX of the GUI more users should begin to run their own nodes.

  - Hard to quantifiy that this would be changes made on Bitcoin Core, espeically so considering UX friendly node tools like Umbrel also use core.

## Current Projects
Below are some design projects I have been working on for Bitcoin Core. Many of these mini-projects have been broken up into smaller versions to limit technical debt and align with the conservative and incremental way in which Bitcoin Core is updated. Lower versions are mostly aimed around content re-works, such as educating users (e.g. clarifying wallet types when creating a wallet), whilst later versions focus more on implementing a new feature (e.g. UI/UX for HWI when creating a wallet). All projects will go through regular reviews via the core GUI repo as well as on the Bitcoin Design Slack. 

### Bitcoin Core design system v1.0

v1.0 will focus on branding and content guidelines as well as provide a resources library for things like figma files, templates, a glossary, guides, presentation kits and designer workflows.

Aiming to develop this design system using [catalog](https://www.catalog.style/). I have started developing this and will create a repo anyone can contribute to soon. I chose catalog because is quite intiutative to use so non-technical designers should not have an issue contributing. Furthermore, many designers are also familiar with web frame works like React (which Catalog is written in) making more technical changes easier to do.

### [GUI on-boarding designs v1.0](https://github.com/bitcoin-core/gui/issues/81)

The aim of this design was to create a high impact, low technical debt design to assist with educating users about the GUI and what it offers. The current on-boarding process is almost non-existant and unclear as to what it is the user is is doing / needs to do. 

### [GUI create wallet designs v1.0](https://github.com/bitcoin-core/gui/issues/77#issue-687141626)     

- 

### [Bitcoin Core Figma file](https://www.figma.com/file/FJ02rY3m8V9ZCDvoXjW39W/Bitcoin-Core?node-id=25%3A569)

I have been working on establishing a 'master' Bitcoin Core figma file that will house things like a designer getting started guide, GUI styleguide, designer workflows, screenshots of various elements of the GUI. I will likely create a new 'Bitcoin Core' figma account to house the above file rather than have it under my own account - governence around this (or if this is even the correct way to go about this) needs to be clarified. 

The basic structure of the design workflow will be: find a problem to solve -> extensively research problem (GH, SE, bitcointalk etc.) -> mock up designs / prototypes in a mixin file of the master figma file (see below) -> some basic user testing -> opening an issue on Github with testing results / rationale -> Iterating designs based on feedback.

One way in which I see designers contrbuting (which will be part of the design workflow) is to make a mixin of the master file (mixins are part of the figma community beta) in which they will work on their designs in following the styleguide / workflow outlined in the master file. This way we can keep track of every individual / file that is being worked on quite easily. 

### Develop design documentation

Develop a design_process.md file to merge into core, similar to the translation_process.md file which outlines how to contribute translations to core. This will be a blend of the design workflow as well as some general GH housekeeping rules to follow. 

Icon policy documentation on how to contribute / implement icons into the GUI repo - this will be for both developers and designers. 

Design workflow documentation. This will be included in GH, figma and the design system. 

### Develop designer guides

A designer focused guide is on assisting designers compile the Bitcoin Core GUI from source and review design changes. [Link to WIP](https://medium.com/p/1e73f478a799/edit). 


## Planned / early stage projects

### Bitcoin Core design system v2.0

This will build on v1.0 and focus on components and patterns as well as foundations like colors, iconography, accessibility and typography. I am currently holding off working on these aspects due to the discussions being had around switching from [Qt Widgets to Qt QML](https://github.com/bitcoin/bitcoin/pull/16883) which have very different design constraints and will determine what direction to take for these parts of the design system. 

### GUI on-boarding designs v2.0

### GUI create wallet designs v2.0

### GUI internal designs for HWI

### GUI multisignature designs

### GUI CoinControl re-design

### Contribute to open-design section of Bitcoin Design Guide

### Re-design bitcoincore.org applying what I develop with the Bitcoin Core Design system v1.0

### Develop user guides
