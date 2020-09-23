# Bitcoin-Core-Design-Foundations [WIP] 

Currently there lacks design foundations within Bitcoin Core making it difficult on-boarding new designers as well as intergrating developers into the design process. This has created a catch-22 situation for contributing designs to Bitcoin Core, as designers are unlikely to create designs if there is no developer to implement them and vice versa for developers implementing designs with limited designer guidance. Establishing some design foundations will help remediate this issue and ultimately result in making software such as the Bitcoin Core GUI more accessible to your average user.

My design philosophy for core is to find a happy-medium between technical prowess and a clean user experience that beginner users can be intuatively guided through. I do not see core (or more specifially the GUI) as being a flashy product like umbrel or mynode but rather a swiss-army knife of sorts that has various tools that can cater to a wide range of users needs whether very techincal or a complete beginer. The Bitcoin Core community has done / is doing some phenomenal work for Bitcoin and I beileve with good design on their side can be a driving force for implementing new features, terminology and practices to the wider Bitcoin ecosystem.

## Goals
The primary overarching goal is to bridge the gap between the Bitcoin Core community and the Bitcoin Design community by establishing solid foundations that developers and designers can build on top of. 

### General goals
- Establish a design system for Bitcoin Core to:
  - Assist with on-boarding new designers and developers.
  - Streamline the design and development process and contribution.
  
- Contribute incremental, conservative but impactful UI/UX changes to the Bitcoin Core GUI. This will assist with establishing design implementation flows that work for both developers and designers. 
  
- Be an active design focused PR reviewer for the Bitcoin Core GUI repo.

- Keeping dialogues going between developers and designers around UI/UX decisions. Core moves at a slow pace so it's easy for certain suggestions to get forgotten over time. 

- Represent end users in many conversations on Github / IRC / Slack that shape the Bitcoin Core GUI. 

- Collaborate with Bitcoin Core design researchers such as Jamaal when it comes to making design decisions. [Jamaal’s Project Horizon.](https://docs.google.com/document/d/1Z2D1Wn5tkQ-Scdp0n8qm2mnFvik1wnU3vcu1DZ1f9jo/edit#)

- Apply what I learn working on designs with Bitcoin Core to the [Bitcoin Design Guide.](https://github.com/BitcoinDesign/Guide)
  - An example being the section on Open Design. I'd imagine insight gained from implementing designs with the Core developers will be useful.

### Specific goals

- Increase Bitcoin Core node count to ~20k by end of 2021 (currently around ~10k). Bitcoin Core is still the primary Bitcoin node software. By improving the UI/UX of the GUI more users should begin to run their own nodes.
  - Hard to quantifiy that this would be changes made on Bitcoin Core, espeically so considering UX friendly node tools like Umbrel also use core.

## Timeline
I'm confident in establishing solid design foundations for Bitcoin Core over the next 6 months. The implementation of specific designs is harder to gauge as its restricted to the pace of Core which historically is quite conservative (for good reason!). In general though it is common for design decisions to be ahead of development changes, I will keep making / improving on designs and hopefully they will eventually get picked up / assist with making a superior design. This document will likely grow larger as time goes on and more ideas surface but this is what I have in the works currently.   

## Current Projects
Below are some design projects I have been working on for Bitcoin Core. Many of these mini-projects have been broken up into smaller versions to limit technical debt and align with the conservative and incremental way in which Bitcoin Core is updated. Lower versions are mostly aimed around content re-works, such as educating users (e.g. clarifying wallet types when creating a wallet), whilst later versions focus more on implementing a new feature (e.g. UI/UX for HWI when creating a wallet). All projects will go through regular reviews via the core GUI repo as well as on the Bitcoin Design Slack. 

### Bitcoin Core design system v1.0
A design system will be pivitol in on-borading new designers and making the design implementation process more seamless. v1.0 will only focus on branding and content guidelines as well as provide a resources library for things like figma files, templates, a glossary, guides, presentation kits and designer workflows.

Aiming to develop this design system using [catalog](https://www.catalog.style/). I have started developing this and will create a repo anyone can contribute to soon. I chose catalog because is quite intiutative to use so non-technical designers should not have an issue contributing. Furthermore, many designers are also familiar with web frame works like React (which Catalog is written in) making more technical changes easier to do.

### [GUI on-boarding designs v1.0](https://github.com/bitcoin-core/gui/issues/81)
The aim of this design was to create a high impact, low technical debt design to assist with educating users about the GUI and what it offers. The current on-boarding process is almost non-existant and unclear as to what it is the user is is doing / needs to do. 

### [GUI create wallet designs v1.0](https://github.com/bitcoin-core/gui/issues/77#issue-687141626)     
- HWI is a top priority.

### Misc designs
Here are some minor design decions I have made / in the process of making. Please view my Github for a deeper dive on discussions / suggestions I've made.

- Added a Tor icon for when all network connections are through the Tor network - [issue](https://github.com/bitcoin-core/gui/issues/58) / [PR](https://github.com/bitcoin-core/gui/pull/86)

- Some minor changes to the create wallet section of the GUI - https://github.com/bitcoin-core/gui/pull/96

### [Bitcoin Core Figma file](https://www.figma.com/file/FJ02rY3m8V9ZCDvoXjW39W/Bitcoin-Core?node-id=25%3A569)

I have been working on establishing a 'master' Bitcoin Core figma file that will house things like a designer getting started guide, GUI styleguide, designer workflows, screenshots of various elements of the GUI. I will likely create a new 'Bitcoin Core' figma account to house the above file rather than have it under my own account - governence around this (or if this is even the correct way to go about this) needs to be clarified. 

The basic structure of the design workflow will be: find a problem to solve -> extensively research problem (GH, SE, bitcointalk etc.) -> mock up designs / prototypes in a mixin file of the master figma file (see below) -> some basic user testing -> opening an issue on Github with testing results / rationale -> Iterating designs based on feedback.

One way in which I see designers contrbuting (which will be part of the design workflow) is to make a mixin of the master file (mixins are part of the figma community beta) in which they will work on their designs in following the styleguide / workflow outlined in the master file. This way we can keep track of every individual / file that is being worked on quite easily. 

### Develop design documentation

Develop a design_process.md file to merge into core, similar to the translation_process.md file which outlines how to contribute translations to core. This will be a blend of the design workflow as well as some general GH housekeeping rules to follow. 

Icon policy documentation on how to contribute / implement icons into the GUI repo - this will be for both developers and designers. 

Design workflow documentation (structure mentioned above). This will be included in GH, figma and the design system. 

### Develop designer guides

A designer focused guide is on assisting designers compile the Bitcoin Core GUI from source and review design changes. [Link to WIP](https://medium.com/p/1e73f478a799/edit). 

### Opening / keeping dialogues going with developers around UI/UX
There are many obvious UX improvements that could be made to core, however the trade-offs are often too great (currently, anyways) or do not align with Bitcoin Core's values. Even if these ideas will never be feasible, it's important to have historical context on these topics so that future designers getting involved do not repeat the same questions. Below are some discussions I've started / will start that may or may not be feasible but are worth being discussed for future reference. This list will grow as time goes on. I will summarise these and future discussions here as well as on the Bitcoin Stack exchange and Bitcointalk where relevant. 

- [Branding](https://github.com/bitcoin-core/gui/issues/89) of Bitcoin Core discussion.

- Creating a design system for Bitcoin Core - this is something that needs to be an on-going discussion between developers and designers.

- Splitting the GUI / CLI into seperate binaries. End users don't need the CLI so why should they download it? An example of a project that does this is [Monero](https://www.getmonero.org/downloads/). 

- Shipping the GUI with Tor binaries that execute on launching. Currently users need to have Tor running before the 'default Tor mode' works out of the box. Many users are likely to not have Tor downloaded but turn on the default Tor option giving them a false sense of privacy. Shipping with the GUI would improve UX around this. 

- Creating a design issue template for the GUI repo. This will help designs provide the right info so they get appropriate feedback from the community, especially developers. As the GUI grows

- Switching from Qt Widgets to Qt QML for the GUI. Qt widgets has many design restraints that make it difficult for desginers to make changes to. Switching to QML gives more flexibility design wise. Furthermore, widgets incurs more technical debt as many changes will be OS specific and make look bad on other OS's requiring much more testing / revewing / desiging. 

- Having HWI installed with the GUI binaries. Currently users have to install this seperately and set the HWI path in the GUI settings. This is quite cumbersome, having HWI installed alongside the GUI and the path automatically set behind the scenes would be ideal. 


## Planned / early stage projects

### Bitcoin Core design system v2.0

This will build on v1.0 and focus on components and patterns as well as foundations like colors, iconography, accessibility and typography. I am currently holding off working on these aspects due to the discussions being had around switching from [Qt Widgets to Qt QML](https://github.com/bitcoin/bitcoin/pull/16883) which have very different design constraints and will determine what direction to take for these parts of the design system. 

### GUI on-boarding designs v2.0
v2.0 will focus on implementing a create wallet flow alongside setting up your node in v1.0. This will include a HWI, which I see as a top priority for the GUI, and the ability to make watch-only wallets by importing descriptors.  

### GUI create wallet designs v2.0

### GUI internal designs for HWI
This will likely occur in parallel to v2.0 of the create wallet designs which integrates HWI UI when creating a wallet. This will include things like signing tx's within the GUI using a hardware wallet. 

### GUI Qt QML designs
This is a major project that will likely involve a big face lift of the GUI. However, switching to QML from widgets is still being discussed so this is on hold until that discussion unfolds. ([WIP PR](https://github.com/bitcoin/bitcoin/pull/16883)). It's likely I will have the design system fleshed out by the time serious QML integration begins which I will apply to these designs. 

### GUI multisignature designs
Once I have the basic create wallet flow UI with HWI developing multisig UI is my next priorirty. 

### GUI CoinControl re-design
Some great discussions and work happening over at the Bitcoin Design community on improving CoinControl UX. Will be implementing this work into the GUI once it is more established - https://github.com/BitcoinDesign/Guide/issues/22. 

### Make an icon library for the GUI
This is a project I will likely collaborate with the Bitcoin design community on. The primary aim is to create an open source icon library that Bitcoin Core, as well as other Bitcoin wallets, can use. Ideally it would be great to have this as its own repo in Bitcoin Core that people can easily clone / modify outside of the GUI repo. 

### Do design work on bitcoincore.org
The user journey does not start once the user downloads the GUI but rather the website its downloaded from, or rather how the user gets to the website itself. I will be applying the Bitcoin Core design system to the website a long with making it more clear what it is the GUI offers (currently it is isn't quite clear on the site). 

### Develop user guides
The GUI can be complicated for users to navigate and some features are still primarily RPC based. I will be creating simple how-to guides for certain features of the GUI that will give simple explanations for technical topics. I will create a list below as I develop and publish ideas. 

### Contribute to open-design section of Bitcoin Design Guide

