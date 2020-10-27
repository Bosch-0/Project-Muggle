![banner image](https://github.com/Bosch-0/Project-Muggle/blob/master/assets/images/bannerimage.png "Banner Image")

## 🧙‍ What is Project Muggle? 
Project Muggle is an initiative started in the [Bitcoin Design community](https://github.com/BitcoinDesign) to improve the user experience of products developed by the [Bitcoin Core project](https://bitcoincore.org/). The Bitcoin Core project maintains and releases an open source Bitcoin client called “[Bitcoin Core](https://github.com/bitcoin).” Bitcoin Core is (currently) the primary reference implementation for the digital currency Bitcoin (BTC).  

The Bitcoin Core project currently has very litte design focused contributors. One way to encourage more designers to contribute to Core is by establishing some design foundations. Foundations will help on-board new designers to the project and help streamline the design process. It will also give guidance to developers and the wider community by establishing design proccesses that should be followed - much like how contributing code has quite established procedures. The Bitcoin Core project has never had a strong design focus resulting in products such as their node/wallet GUI lacking much needed design direction. Having design foundations will save time and resources by limiting developmental debt - both in terms of technical and design.



## 🏆 Goal of Project Muggle 
Establish design foundations for the Bitcoin Core project over the next 6 months (as of November 2020). Bitcoin has yet to break out of the non-magical community (programming wizards) into the world of ordinary human beings (muggles). With good design, which starts with solid design foundations, this bridge can be gapped making the magical internet money known as bitcoin more accessible to muggles. 

This repo will keep track of efforts made in establishing these foundations. It will be periodically updated. If you wish to collaborate on Project Muggle reach out to me on the [Bitcoin Design Slack](https://bitcoindesign.slack.com/join/shared_invite/zt-gytq2snl-4TEWJOTKrXRCB4YLBoDunA#/) or [twitter](https://twitter.com/_bosch_). 


---



## 🌌 The Bitcoin Core project design system 
A design system has many definitions. But, I am quite fond of the Nielsen Norman Group's definition below:

> Design Systems—also known as 'pattern libraries' or 'component  libraries'—promote quality, consistent UX design across products; and  expedite the work of designers, developers, and anyone else working on a  website, application, or any digital design.

Design systems may also cover topics such as branding, content and resources. [Atlassian's design system](https://atlassian.design/) is an example of a more comprehensive design system.

A design system is design foundations in and of itself. Much of the projects below this will feed back into this design system. Having a design system will be pivotal in on-boarding new designers. A design system will make developing, contributing and testing designs more seamless.

A basic [design system](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Bitcoin-Core-Design-System?node-id=271%3A527) is being built on Figma hosted by a [Bitcoin Core Figma account](https://www.figma.com/@BitcoinCore). This Figma native design system will establish guidelines for designers wanting to contribute to Bitcoin Core. How best to go about governance of this account needs to be clarified. Ideally it will be stored as a .fig file in bitcoin-core/gui and updated through community consensus. Design contributors can also remix the design system file as a pseudo-version control.



## 🛠️ GUI pull request (PR) testing
A major development bottleneck for the Bitcoin Core project is the limited amount of PR testers / reviewers. This issue is amplified for the GUI which is primarily manually tested. Like code, designs should be heavily peer reviewed. This is especially so for a security focused project like Bitcoin Core with mistakes possibly resulting in a huge loss of funds. Currently, Bitcoin Core has few design focused contributors. Having design foundations established will help on-board designers. It will also assist developers understand the design process. 

To assist with establishing workflows and bridging the designer / developer gap I will be an active design focused GUI PR tester. Insights gained by actively being involved in the development process will be valuable in establishing design foundations for core as well as be useful for the wider Bitcoin community (such as applying what I learn to the Bitcoin Design guide). Additionally, I'll be aiming to get more designers and non-designers testing PRs through user friendly guides (see documentation section below) and offer assistance to those interested.



## 🔬 Research
The Bitcoin Core wallet (GUI / CLI) offers a range of UX constraints not seen in conventional Bitcoin wallets. An example being the use of hardened hierarchical deterministic wallets. This makes it unable to export xpubs making things like setting up a multisig wallet using Bitcoin Core GUI as a signer difficult. Another example is Bitcoin Core's lack of support of BIP39 mnemonics, causing many interoperability issues with other wallets. Though these are not unfounded decisions and in practically all cases have been done to increase security. Due to the unique nature of the Bitcoin Core wallet, designers must build UI/UX from the ground up working within these constraints. I will be actively researching how to best go about maximixing UX in the Bitcoin Core wallet within these technical constraints. My aim is to have Bitcoin Core be a refernce implemenation for UI/UX best practices when desiging a Bitcoin wallet like Bitcoin Core. 

A recent square crypto design grantee Jamaal is [conducting design research](https://docs.google.com/document/d/1Z2D1Wn5tkQ-Scdp0n8qm2mnFvik1wnU3vcu1DZ1f9jo/edit#) around who uses the Bitcoin Core wallet. I'll be actively collaborating with Jamaal were relevant.

Research is also being conducted by the Bitcoin Design community in establishing a Bitcoin Design guide. I'll be actively applying insights relevant to the design of Bitcoin Core. 



## 📙 Contribute to Bitcoin Design Guide
Insights gained whilst building design foundations for Bitcoin Core will be contrbiuted to the open source [Bitcoin Design Guide](https://github.com/BitcoinDesign/Guide). 

> The Bitcoin Design Guide is a free open-source community resource that helps designers, developers and others working on non-custodial bitcoin-products to create better experiences, faster. We hope that, over time, it will cover all relevant types of products, including consumer wallets, merchant interactions, exchanges and more. Better products and experiences should ultimately make it more appealing for anyone to own and use bitcoin.



## 🎨 Design work

- Work on designs on other open source Bitcoin projects for more rapid prototyping for core.
- Testing workflows that will feed into design system.
- A project like Bitcoin Core needs incremental, minor design additions to prevent too much overhead but avoid being too small to prevent bikeshedding. Bikeshedding at the beginning will likely occur while design proccesses are worked out. 



### Open source bitcoin icon library
The primary aim of this project is to create an open source bitcoin centric icon library that projects like Bitcoin Core can use in their applications. This will likely be an open initiative that project muggle and the Bitcoin Design community will work on.

[Link to repo](https://github.com/Bosch-0/Bitcoin-Icons)



### Bitcoincore.org
The user journey does not start once the user downloads the GUI but rather the website its downloaded from. Whilst applying the Bitcoin Core design system I aimt to improve the UI/UX of bitcoincore.org to better assist end users on the journey on using the GUI. 

Cobra (owner or bitcoin.org) is working on a [Bitcoin wallet](https://twitter.com/cobrabitcoin/status/1310304498125025282?s=21) which could mean a conflict of interest when it comes to recommending wallets on bitcoin.org. With Re-desigining bitcoincore.org I am aiming for bitcoincore.org to be the primary place for end users to download the Bitcoin Core GUI.



### QML based GUI
This is a major project that will involve a big face lift of the GUI. Switching to Qt QML from Qt widgets (details above) is still being discussed so work on this is on hold until that discussion unfolds. ([WIP PR](https://github.com/bitcoin/bitcoin/pull/16883)). It's likely I will have the design system established by the QML integration (if it happens) which I can apply to the QML designs. Below are some rough ideas that I will be exploring for this design:

- Aiming to design a very minimilist, monochrome, to the point application. I think this aligns well with the neutral and conservative nature of the Bitcoin Core community. 



### GUI onboarding wizard
Currently the Bitcoin Core GUI has a limited onboarding process. Onboarding is a crucial step for any digital app to educate the users about the product. Currently users are thrown into the GUI with little guidance. The Bitcoin Core GUI has many features that can be confusing to new users. A well crafted onboarding process can help clarify these features for users. 

The onboarding designs are broken up into versions. This limits technical overhead making it easier for developers to implement designs. Core moves in calculated and incremental steps so atomizing these designs makes sense. 

[Version 0.1](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=1%3A15)
Version 0.1 reworks the current limited onboarding. It focuses on educating the user about the GUI and running a node. 

**INSERT IMAGE**
  
[Version 0.2](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=5%3A502)
Version 0.2 will add to 1.0 by introducing a basic create wallet flow to the onboarding process. This wallet flow may include HWW integration depending [if its merged](https://github.com/bitcoin-core/gui/pull/4). 



### GUI create wallet flow
The current create wallet user flow does little to educate the user about what it is they are doing. Creating a wallet is an important action all Bitcoin users undertake. Wallet creation comes with many caveats and intricacies. Without educating users through the process it's likely they will costly errors.

[Version 0.1](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=5%3A1)
Version 0.1 focuses on re-working the current content. This is to make it more clear to users about what they actions they are taking / trade offs they are making. This version has been shared on GitHub for feedback [issue #77](https://github.com/bitcoin-core/gui/issues/77#issue-687141626)

[Version 0.2](#)
Version 0.2 focuses on adding extra features to the basic create wallet flow. Examples include HWW integration and descriptor imports. 



### GUI CoinControl
[Some great discussions](https://github.com/BitcoinDesign/Guide/issues/22) and work happening over at the Bitcoin Design community on improving CoinControl UX. Will be implementing these insights from here into the GUI's currently coin control UI.



### GUI HWI UI
This will likely occur in parallel to v2.0 of the create wallet designs which integrates HWW UI when creating a wallet. This will include things like signing tx's within the GUI using a hardware wallet.  



### GUI multisig UI 
Once the GUI has a basic HWW create wallet flow UI implemented, multisig UI is the next priority. Multisig in Bitcoin Core is quite different from other wallets (due to no BIP39 implementation) so this will need to be designed from the ground up. 



### GUI descriptor UI 
Descriptor wallets which are included in the next major Bitcoin Core release (0.21) offer a wide range of UX implications. There does not yet exist any reference UI/UX best practices for working with descriptors so this project will involve quite a bit of research. Some examples of UX improvements descriptors can offer are below:

- Easier multisig backups.
- Better wallet management. 
 


## 📄 Documentation / Guides

### Documentation
text here

- design_process.md for the bitcoin-core/gui repo. This will give guidance to designers contributing designs to Bitcoin Core. 
- [Icon_policy.md](https://docs.google.com/document/d/1jXWwXM71_t7zIBlTu2aOzvhGj0ZWyml_yXXzuXMHLSg/edit) on how to contribute icons to Bitcoin Core. 
- [Design workflows](https://www.figma.com/file/si2C2uAPyGUHrvdnkJtmI5/Bitcoin-Core-Figma-Workflow?node-id=718%3A369).


### Designer Guides
Guides will be published on Medium whilst I build my personal site (coming soon).

- Compiling the Bitcoin Core GUI from source for designers.
([Windows](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-windowsos-1e73f478a799), [macOS](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-macos-7ef2e1c6d8b0), [Linux](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-linux-936ed2fca125)).
- Create design issue template for bitcoin-core/gui. 

### User guides
The GUI can be complicated for users to navigate and some features are still primarily RPC based. I aim to create simple how-to guides for certain features of the GUI that will give simple explanations for technical topics. I will create a list below as I develop and publish ideas. 

- Setting up your Bitcoin Core node 
- Generating a multisig wallet on Bitcoin Core
- Connecting you Bitcoin Core node over Tor 


## 🗯️ Design discussions
Below are discussions started / will be started that may or may not be feasible but are worth being discussed for future reference. Discussions will be had on various platforms such as GitHub, StackExchange and Bitcointalk, links will be included to each. Outside of the scope of the below discussions I will aim to represent the end users in discussions on various platforms. 

- [Bitcoin Core Branding](https://github.com/bitcoin-core/gui/issues/89).
- Bitcoin Core design system. 
- Switching from Qt Widgets to a Qt QML GUI.
- Are desktop nodes relevant?
- Switching net's within the gui [issue #78](https://github.com/bitcoin-core/gui/issues/78)
- Splitting the GUI / CLI into separate binaries.
- [Bitcoin Core / Research the history of Core GUI changes through Github issues](https://github.com/BitcoinDesign/Meta/issues/19) 
- Having HWI installed with GUI binaries.
- Tor binaries shipped with GUI.



## 🤏 Minor design contributions
Minor design contributions. These assist with establishing solid designer and developer workflows. 

- Added Tor icon to GUI [issue #58](https://github.com/bitcoin-core/gui/issues/58) / [PR #86](https://github.com/bitcoin-core/gui/pull/86)
- Minor changes to the create wallet section of the GUI [PR #96](https://github.com/bitcoin-core/gui/pull/96)
- Privacy mode toggle option [issue #82](https://github.com/bitcoin-core/gui/issues/82)
- More informative tray icons [issue #70](https://github.com/bitcoin-core/gui/issues/70)
