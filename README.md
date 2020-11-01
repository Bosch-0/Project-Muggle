![banner image](https://github.com/Bosch-0/Project-Muggle/blob/master/assets/images/bannerimage.png "Banner Image")

# 🧙‍ What is Project Muggle? 
Project Muggle is an initiative started in the [Bitcoin Design community](https://github.com/BitcoinDesign) to improve the design focus of applications developed by the [Bitcoin Core project](https://bitcoincore.org/). The Bitcoin Core project maintains and releases the open source Bitcoin client called “[Bitcoin Core](https://github.com/bitcoin).” Bitcoin Core is (currently) the primary reference implementation for the digital currency Bitcoin (BTC).  

Bitcoin has yet to break out of the non-magical community (programming wizards) into the world of ordinary human beings (muggles). Design is one way to help bridge this gap and make the magical internet money known as bitcoin more accessible to the average person.

This repo will keep track of efforts made in improving the design focus of Bitcoin Core. If you wish to collaborate on Project Muggle reach out on the [Bitcoin Design Slack](https://bitcoindesign.slack.com/join/shared_invite/zt-gytq2snl-4TEWJOTKrXRCB4YLBoDunA#/) or [twitter](https://twitter.com/_bosch_). 



# 🏆 Goal of Project Muggle 
Establish design foundations and direction for Bitcoin Core by the 0.22.0 release (~July 2021). 

<details>
 <summary> What will this achieve?</summary>

- Better UI/UX for current and future users of Bitcoin Core products such as the GUI / website. 
- More design focused contributors.
- Stronger design focus in the contribution process. 
- Save time and resources by reducing  developmental debt - both technical and design.
</details> 



# What is Project Muggle working on? 
## 🌌 Bitcoin Core Design system(s)
A design system has many definitions, though the Nielsen Norman Group's definition below is quite accurate:

> Design Systems—also known as 'pattern libraries' or 'component  libraries'—promote quality, consistent UX design across products; and  expedite the work of designers, developers, and anyone else working on a  website, application, or any digital design.

Project Muggle will initially establish two Figma native design systems for Bitcoin Core. One for the [GUI](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/GUI-Design-System?node-id=1830%3A608) and one for [bitcoincore.org](https://www.figma.com/file/k30cNrPIUybQ8rpvuDF60Q/Website-Design-System?node-id=6%3A0). These two files will be hosted by the [BitcoinCore Figma account](https://www.figma.com/@BitcoinCore). Having a design system will be assist in on-boarding new designers and will significantly speed up the developing, contributing and testing of designs.

Two will exist initially due to the constraints of the Qt widgets framework currently used by the GUI  which uses native OS styling making a custom design system challenging. The GUI design system will be built around these constraints while the bitcoincore.org design system will introduce a whole new custom look and feel. It's likely the GUI will transition to using the more flexible Qt framework QML (discussions currently underway) in the near future of which the design system built for bitcoincore.org will be applied to a new custom QML based design. 

The design systems will be built along side other initatives Project Muggle is working on. 

To see how designers will work with these design systems a README at the start of each design system outlining the workflow has been included.

A single, full fledged design system including design and code snippets will eventually be hosted on GitHub pages through a live, interactive web app.



## 🌐 Bitcoincore.org redesign 

The user journey does not start once the user downloads the GUI but rather the website its downloaded from. Whilst applying the Bitcoin Core design system I aim to improve the UI/UX of bitcoincore.org to better assist end users on the journey on using the GUI. 

Cobra (owner or bitcoin.org) is working on a [Bitcoin wallet](https://twitter.com/cobrabitcoin/status/1310304498125025282?s=21) which could mean a conflict of interest when it comes to recommending wallets on bitcoin.org. With Re-desigining bitcoincore.org I am aiming for bitcoincore.org to be the primary place for end users to download the Bitcoin Core GUI.



## 🟠 Open source Bitcoin icon library
The primary aim of this project is to create an open source bitcoin centric icon library that projects like Bitcoin Core can use in their apps. This will likely be an open initiative that Project Muggle and the Bitcoin Design community will collaboratively work on.

[Link to repo](https://github.com/Bosch-0/Bitcoin-Icons)



## 📙 Contribute to Bitcoin Design Guide
Project Muggle will contribute to the open source [Bitcoin Design Guide](https://github.com/BitcoinDesign/Guide) were relevant. 

> The Bitcoin Design Guide is a free open-source community resource that helps designers, developers and others working on non-custodial bitcoin-products to create better experiences, faster. We hope that, over time, it will cover all relevant types of products, including consumer wallets, merchant interactions, exchanges and more. Better products and experiences should ultimately make it more appealing for anyone to own and use bitcoin.



## 🛠️ Bitcoin Core GUI pull request (PR) testing
A major development bottleneck for the Bitcoin Core project is the limited amount of PR testers. This issue is amplified for the GUI which needs to be tested accross various operating systems manually. Additionaly, Bitcoin Core has few design focused testers / contributors resulting in the design of many PRs mostly being an afterthought or unfounded in design principlies. 

To assist with bridging the designer / developer gap I (Bosch) will be actively testing GUI PRs as part of Project Muggle. More specifically I will give design guidance on PRs alongside testing for bugs. Insights gained through testing PRs will be valuable in establishing design procedures for Bitcoin Core, as well as be useful for the wider Bitcoin community (such as contributing to the Bitcoin Design Guide). 

Project Muggle will also be aiming to encourage more users (designers or not) to start testing PRs with well designed guides and documentation (see guides and documentation sections below).



## 🔬 Research
The Bitcoin Core wallet has a range of novel features not present in conventional Bitcoin wallets. Project Muggle will be conducting design research as how best to devlelop the UI/UX of the Bitcoin Core wallet within these constraints.

Project Muggle will actively collaborate with Bitcoin Core wallet research project, [Project Horizon](https://docs.google.com/document/d/1Z2D1Wn5tkQ-Scdp0n8qm2mnFvik1wnU3vcu1DZ1f9jo/edit#) on who the users of the Bitcoin Core wallet are were relevant. Project Muggle will also be working alongside the Bitcoin Design community throughout its research.

<details>
  <summary>Research areas of interest</summary>
  
- Desigining for Bitcoin Core post 0.21.0 - Taproot, MuSig, descriptors and more.
- UX friendly wallet backups without BIP39.
- Multisig / HWI intergration with hardened hierarchical Deterministic Wallets.
- Node bootstrapping.
</details>



## 🖥️ GUI Designs


### QML Version
This is a major project that will involve a big face lift of the GUI. Switching to Qt QML from Qt widgets (details above) is still being discussed so work on this is on hold until that discussion unfolds. ([WIP PR](https://github.com/bitcoin/bitcoin/pull/16883)). It's likely I will have the design system established by the QML integration (if it happens) which I can apply to the QML designs. Below are some rough ideas that I will be exploring for this design:

- Aiming to design a very minimilist, monochrome, to the point application. I think this aligns well with the neutral and conservative nature of the Bitcoin Core community. 


### Onboarding wizard
Currently the Bitcoin Core GUI has a limited onboarding process. Onboarding is a crucial step for any digital app to educate the users about the product. Currently users are thrown into the GUI with little guidance. The Bitcoin Core GUI has many features that can be confusing to new users. A well crafted onboarding process can help clarify these features for users. 

The onboarding designs are broken up into versions. This limits technical overhead making it easier for developers to implement designs. Core moves in calculated and incremental steps so atomizing these designs makes sense. 

<details>
  <summary>Version 0.1</summary>
  
  
Version 0.1 reworks the current limited onboarding. It focuses on educating the user about the GUI and running a node. [Link](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=1%3A15) to active design work.

**INSERT IMAGE**

</details>
 
 <details>
   <summary> Version 0.2 </summary>
 
Version 0.2 will add to 0.1 by introducing a basic create wallet flow to the onboarding process. This wallet flow will include HWW integration depending [if its merged](https://github.com/bitcoin-core/gui/pull/4). [Link](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=104%3A216) to active design work.
 
 </details>
 

### Create wallet flow
The current create wallet user flow does little to educate the user about what it is they are doing. Creating a wallet is an important action all Bitcoin users undertake. Wallet creation comes with many caveats and intricacies. Without educating users through the process it's likely they will costly errors.

[Version 0.1](https://www.figma.com/file/4dO1LqPY0WAgp5d1Bz3U8j/Bitcoin-Core-Designs?node-id=5%3A1)
Version 0.1 focuses on re-working the current content. This is to make it more clear to users about what they actions they are taking / trade offs they are making. This version has been shared on GitHub for feedback [issue #77](https://github.com/bitcoin-core/gui/issues/77#issue-687141626)

[Version 0.2](#)
Version 0.2 focuses on adding extra features to the basic create wallet flow. Examples include HWW integration and descriptor imports. 


### CoinControl
[Some great discussions](https://github.com/BitcoinDesign/Guide/issues/22) and work happening over at the Bitcoin Design community on improving CoinControl UX. Will be implementing these insights from here into the GUI's currently coin control UI.


### Hardware wallet intergration
This will likely occur in parallel to v2.0 of the create wallet designs which integrates HWW UI when creating a wallet. This will include things like signing tx's within the GUI using a hardware wallet.  


### Multisig 
Once the GUI has a basic HWW create wallet flow UI implemented, multisig UI is the next priority. Multisig in Bitcoin Core is quite different from other wallets (due to no BIP39 implementation) so this will need to be designed from the ground up. 


### Descriptors
Descriptor wallets which are included in the next major Bitcoin Core release (0.21) offer a wide range of UX implications. There does not yet exist any reference UI/UX best practices for working with descriptors so this project will involve quite a bit of research. Some examples of UX improvements descriptors can offer are below:

- Easier multisig backups.
- Better wallet management. 
 


## 📄 Documentation
text here

- [design_process.md](https://github.com/Bosch-0/Project-Muggle/blob/master/docs/design_process.md) for how to contribute designs to Bitcoin Core.
- [icon_policy.md](https://github.com/Bosch-0/Project-Muggle/blob/master/docs/icon_policy.md) on how to contribute icons to Bitcoin Core. 



## 🗺️ Guides
Guides will be published on Medium / GitHub and my personal site (coming soon).

### Designer guides
- Compiling the Bitcoin Core GUI from source for designers.
([Windows](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-windowsos-1e73f478a799), [macOS](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-macos-7ef2e1c6d8b0), [Linux](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-linux-936ed2fca125)).
- Create design issue template for bitcoin-core/gui. 

### User guides
Project Muggle creates simple how-to guides to help end users navigate products developed by Bitcoin Core such as the GUI. 

<details>
 <summary> List of user guides</summary>
 
- Setting up your Bitcoin Core GUI node.
- Generating a multisig wallet on the Bitcoin Core GUI.
- Connecting you Bitcoin Core GUI node over Tor.
 
</details>



## 🗯️ Design discussions
Project Muggle aims to actively keep design dialogues going between the Bitcoin Core community, developers and designers. 

<details>
  <summary>Discussions</summary>

- [Bitcoin Core Branding](https://github.com/bitcoin-core/gui/issues/89).
- [Bitcoin Core / Research the history of Core GUI changes through Github issues](https://github.com/BitcoinDesign/Meta/issues/19) 
- Switching net's within the gui [issue #78](https://github.com/bitcoin-core/gui/issues/78)
- Establishing a Bitcoin Core design system. 
- Switching Qt framework from widgets to QML.
- Headless Bitcoin Core setup.
- Having HWI installed with GUI binaries.
- Tor binaries shipped with GUI.

</details>



## 🤏 Minor design contributions
Minor design contributions.

<details>
  <summary>Below are minor UI/UX contributions Project Muggle has made</summary>
 
- Add Tor icon to GUI [issue #58](https://github.com/bitcoin-core/gui/issues/58) / [PR #86](https://github.com/bitcoin-core/gui/pull/86)
- Slight GUI UX improvement when creating wallets [PR #96](https://github.com/bitcoin-core/gui/pull/96)
- Privacy mode toggle option [issue #82](https://github.com/bitcoin-core/gui/issues/82)
- More informative tray icons [issue #70](https://github.com/bitcoin-core/gui/issues/70)

 </details
