# Establishing Bitcoin Core Design foundations [WIP] 
Bitcoin Core currently lacks design foundations. This has impeded on-boarding designers and integrating the design and development process. With no design foundations, designers are unlikely to contribute designs. Without designers, developers may integrate unfounded design decisions resulting in technical debt. Establishing design foundations will prevent these issues occurring and streamline the design process. 

Like code, designs should be peer reviewed by as many eyes as possible. Currently Bitcoin Core has few design focused contributors. Having design foundations established will help on-board designers. It will also assist developers understand the design process. Having more designer contributors will result in more robust designs. 

This repo will keep track of efforts made in establishing these foundations. It will be periodically updated.

## Goal / timeline
Establish design foundations for Bitcoin Core over the next 6 months (as of October 2020). Below are methods I am emplyoing to acheive this goal.

## Establish a Bitcoin Core design system 
A design system has many definitions. But, I am quite fond of the Nielsen Norman Group's definition below:

> Design Systems—also known as 'pattern libraries' or 'component  libraries'—promote quality, consistent UX design across products; and  expedite the work of designers, developers, and anyone else working on a  website, application, or any digital design.

Design systems may also cover topics such as branding, content and resources. [Atlassian's design system](https://atlassian.design/) is an example of a more comprehensive design system.

A design system is design foundations in and of itself. Much of the action items below this will feed back into this design system. Having a design system will be pivotal in on-boarding new designers. A design system will make developing, contributing and testing designs seamless.

I've chosen to break development of the design system into stages. This is to limit overhead and to work within technical constraints currently in Core. Those being around the GUI and what Qt framework it will use going forward. Currently it uses Qt Widgets which has many operating system design limitations. Qt QML is the alterantive which gives much more design flexibility. Discussions are currently underway regarding switching from [Qt Widgets to Qt QML](https://github.com/bitcoin/bitcoin/pull/16883).

The [design system](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Bitcoin-Core-Design-System?node-id=271%3A527) will be built on Figma hosted by a [Bitcoin Core Figma account](https://www.figma.com/@BitcoinCore). How best to go about governance of this account needs to be clarified. Ideally it will be stored as a .fig file in bitcoin-core/gui and updated through community consensus. Design contributors can also remix the design system file as a pseudo-version control.

### Version 1.0

Version 1.0 focuses on branding, content, workflows and developing resource libraries. Branding will focus on things like mission and personality. As well as offer guidance on how to use assets like the Bitcoin Core logo. Workflows outline processes developers and designers should take when contributing designs to Bitcoin Core. The content section will offer guidelines around language, grammar, and writing style. It will also offer a glossary for definitions of words used by Bitcoin Core. The resources library will include Figma files, templates, guides, presentation kits and much more.

### Version 2.0

Version 2.0 will focus on components, patterns, colors, iconography, accessibility and typography. Work on this version is being held off until the Qt Widgets/QML discussion unfolds some more. Which Qt framework is chosen will impact these sections of the design system. For now the design system will include screenshots of how the GUI looks on Windows, mac and Linux. 

### Design QML based GUI
This is a major project that will likely involve a big face lift of the GUI. However, switching to QML from widgets is still being discussed so this is on hold until that discussion unfolds. ([WIP PR](https://github.com/bitcoin/bitcoin/pull/16883)). It's likely I will have the design system fleshed out by the time serious QML integration begins which I will apply to these designs.

## Design GUI onboarding wizard
Currently the Bitcoin Core GUI has a limited onboarding process. Onboarding is a crucial step for any digital app to educate the users about the product. Currently users are thrown into the GUI with little guidance. The Bitcoin Core GUI has many features that can be confusing to new users. A well crafted onboarding process can help clarify these features for users. 

The onboarding designs are broken up into versions. This limits technical overhead making it easier for developers to implement designs. Core moves in calculated and incremental steps so atomizing these designs makes sense. 

**[Version 1.0](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=1%3A15)**
  
Version 1.0 reworks the current limited onboarding. It focuses on educating the user about the GUI and running a node. 

**IMAGE GOES HERE**
  
**[Version 2.0](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=5%3A502)**

Version 2.0 will add to 1.0 by introducing a basic create wallet flow to the onboarding process. This wallet flow may include HWW integration depending [if its merged](https://github.com/bitcoin-core/gui/pull/4). 

## Redesign GUI create wallet flow
The current create wallet user flow does little to educate the user about what it is they are doing. Creating a wallet is an important action all Bitcoin users undertake. Wallet creation comes with many caveats and intricacies. Without educating users through the process it's likely they will costly errors.

**[Version 1.0](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=5%3A1)**

Version 1.0 focuses on re-working the current content. This is to make it more clear to users about what they actions they are taking / trade offs they are making. This version has been shared on GitHub for feedback [issue #77](https://github.com/bitcoin-core/gui/issues/77#issue-687141626) 

**Version 2.0**

Version 2.0 focuses on adding extra features to the basic create wallet flow. This includes things like HWW integration and descriptor imports. 

### Redesign bitcoincore.org
The user journey does not start once the user downloads the GUI but rather the website its downloaded from, or rather how the user gets to the website itself. I will be applying the Bitcoin Core design system to the website a long with making it more clear what it is the GUI offers (currently it is isn't quite clear on the site).

I'll be taking a development and designer roll for this. For privacy reasons bitcoincore.org should be CSS only (no JS). 

Cobra (owner or bitcoin.org) is also working on a [Bitcoin wallet](https://twitter.com/cobrabitcoin/status/1310304498125025282?s=21) which could mean a conflict of interest when it comes to recommending wallets on bitcoin.org. Re-desigining bitcoincore.org will hopefully result in this being the primary place for end users to download Bitcoin Core binaries.

## Documentation
Write a design_process.md file to merge into core, similar to the translation_process.md file which outlines how to contribute translations to core. This will be a blend of the design workflow as well as some general GH housekeeping rules to follow. 

Icon policy documentation on how to contribute / implement icons into the GUI repo - this will be for both developers and designers. 

[Design workflow documentation](https://www.figma.com/file/si2C2uAPyGUHrvdnkJtmI5/Bitcoin-Core-Figma-Workflow?node-id=718%3A369). This will be included on GitHub, figma and the design system.

## Designer guides
All guides will be moved from Medium to my own self-hosted site soon. They will also be published on my GitHub account within an appropriate repo (likely the Bitcoin Core Design repo mentioned in the Bitcoin Core Figma account discussion above). 

- Compiling the Bitcoin Core GUI from source for designers. One guide for each major OS ([Windows](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-windowsos-1e73f478a799), [macOS](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-macos-7ef2e1c6d8b0), [Linux](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-linux-936ed2fca125)).

- Create a design issue template for GUI repo. This will help designers provide the right details of their designs so they get appropriate feedback from the community, especially developers.

### User guides
The GUI can be complicated for users to navigate and some features are still primarily RPC based. I will be creating simple how-to guides for certain features of the GUI that will give simple explanations for technical topics. I will create a list below as I develop and publish ideas. 

## Design discussions
Many Bitcoin Core design discussions may never go anywhere for various technical / historical / philosophical reasons. However, it's important to have historical context so that future designers getting involved do not repeat the same questions. Below are some discussions I've started / will start that may or may not be feasible but are worth being discussed for future reference. This list will grow as time goes on. Discussions will be had on various platforms such as GitHub, StackExchange and Bitcointalk. Summary's of discussions will be added as they unfold. 

- [Bitcoin Core Branding](https://github.com/bitcoin-core/gui/issues/89).

- Establishing a Bitcoin Core design system. (opening an issue soon) 

- Switching from Qt Widgets to Qt QML for the GUI. Qt widgets has many design restraints that make it difficult for designers to make changes to. Switching to QML gives more flexibility design wise. Furthermore, widgets incurs more technical debt as many changes will be OS specific and make look bad on other OS's requiring much more testing / reviewing / designing. 

- Having HWI installed with the GUI binaries. Currently users have to install HWI separately and set the HWI path in the GUI settings. HWI downloaded and installed as part of the download process may resolve this UX issue. 

- Are desktop nodes the way forward? People generally don't have their desktop running 24/7 like a node should be. Having external hardware that runs the node that a desktop GUI connects to would be ideal. 

- Switching net's within the gui [issue #78](https://github.com/bitcoin-core/gui/issues/78)

- Splitting the GUI / CLI into separate binaries. End users don't need the CLI so why should they download it? An example of a project that does this is [Monero](https://www.getmonero.org/downloads/). 

- Shipping the GUI with Tor binaries that execute on launching. Currently users need to have Tor running before the 'default Tor mode' works out of the box. Many users are likely to not have Tor downloaded but turn on the default Tor option giving them a false sense of privacy. Shipping with the GUI would improve UX around this. 

## Minor design contributions
These are minor design contributions made / in the process of making.

- Added a Tor icon for when all network connections are through the Tor network [issue #58](https://github.com/bitcoin-core/gui/issues/58) / [PR #86](https://github.com/bitcoin-core/gui/pull/86)

- Minor changes to the create wallet section of the GUI [PR #96](https://github.com/bitcoin-core/gui/pull/96)

- Privacy mode toggle option [issue #82](https://github.com/bitcoin-core/gui/issues/82)

- More informative tray icons [issue #70](https://github.com/bitcoin-core/gui/issues/70)
 
### Design GUI internal HWI UI
This will likely occur in parallel to v2.0 of the create wallet designs which integrates HWI UI when creating a wallet. This will include things like signing tx's within the GUI using a hardware wallet.  

### Design GUI multisig UI 
Once I have the basic create wallet flow UI with HWI developing multisig UI is my next priority. 

### Redesign GUI CoinControl
Some great discussions and work happening over at the Bitcoin Design community on improving CoinControl UX. Will be implementing this work into the GUI once it is more established—https://github.com/BitcoinDesign/Guide/issues/22. 

### Make GUI icon library
This is a project I will likely collaborate with the Bitcoin design community on. The primary aim is to create an open source icon library that Bitcoin Core, as well as other Bitcoin wallets, can use.

### Contribute to open-design section of Bitcoin Design Guide
