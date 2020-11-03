![banner image](https://github.com/Bosch-0/Project-Muggle/blob/master/assets/images/bannerimage.png "Banner Image")

# 🧙‍ What is Project Muggle? 
Project Muggle is an initiative started in the [Bitcoin Design community](https://github.com/BitcoinDesign) to improve the design focus of applications developed by the [Bitcoin Core project](https://bitcoincore.org/). The Bitcoin Core project maintains and releases an open source Bitcoin client called “[Bitcoin Core](https://github.com/bitcoin).” Bitcoin Core is (currently) the primary reference implementation for the digital currency Bitcoin (BTC).  

Bitcoin has yet to break out of the non-magical community (programming wizards) into the world of ordinary human beings (muggles). Design is one way to help bridge this gap and make the magical internet money known as bitcoin more accessible to the average person.

This repo will keep track of efforts made in improving the design focus of Bitcoin Core. If you wish to collaborate on Project Muggle reach out on the [Bitcoin Design Slack](https://bitcoindesign.slack.com/join/shared_invite/zt-gytq2snl-4TEWJOTKrXRCB4YLBoDunA#/) or [twitter](https://twitter.com/_bosch_). 



# 🏆 Goal of Project Muggle 
Establish design foundations and direction for Bitcoin Core by the 0.22.0 release (~July 2021). 

### What will this achieve?

- Better UI/UX for current and future users of Bitcoin Core products such as the GUI / website. 
- More design focused contributors / stronger design contribution process within Bitcoin Core.
- Save time and resources by reducing developmental debt - both technical and design.
- Assist with establishing Bitcoin open design processes and standards that help the wider Bitcoin ecosystem. 



# What is Project Muggle working on? 
## 🌌 Bitcoin Core Design system(s)
A design system has many definitions, though the Nielsen Norman Group's definition below is quite accurate:

> Design Systems—also known as 'pattern libraries' or 'component  libraries'—promote quality, consistent UX design across products; and  expedite the work of designers, developers, and anyone else working on a  website, application, or any digital design.

Project Muggle will initially establish two Figma native design systems for Bitcoin Core. One for the [GUI](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/GUI-Design-System?node-id=1830%3A608) and one for [bitcoincore.org](https://www.figma.com/file/k30cNrPIUybQ8rpvuDF60Q/Website-Design-System?node-id=6%3A0). These two files will be hosted by the [BitcoinCore Figma account](https://www.figma.com/@BitcoinCore). Having a design system will be assist with on-boarding new designers and will significantly speed up the developing, contributing and testing of designs.

Two will exist initially due to the constraints of the Qt widgets framework currently used by the GUI which uses native OS styling making a custom design system challenging. The GUI design system will be built around these constraints while the bitcoincore.org design system will introduce a whole new custom look and feel. It's likely the GUI will transition to using the more flexible Qt framework QML (discussions currently underway) in the near future of which the design system built for bitcoincore.org will be applied to a new custom QML based design. 

To see how designers will work with these design systems a [README](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/?node-id=271%3A527) at the start of each design system outlining workflows has been included.

A single, full fledged design system including design and code snippets will eventually be hosted on GitHub pages through a live, interactive web app.



## 🌐 Bitcoincore.org redesign 
Project Muggle will be working on a complete re-design of bitcoincore.org using our Bitcoin Core website design system. 

Bitcoincore.org currently has a dated and not so user friendly design. User journey's do not start with running the application. In the case of the GUI downloading the binaries from a trusted source such as bitcoincore.org is a first step. The current design does not communicate trust nor does it do a good job educating users about Bitcoin Core and what it offers. A re-design that puts emphasis on user experience and trust will significantly improve how users view Bitcoin Core and its associated products. 



## 🟠 Open source Bitcoin icon library
Project Muggle will be developing an open source bitcoin centric icon library that projects like Bitcoin Core can use in their applications. This will be an open initiative that Project Muggle and the wider Bitcoin Design community will collaboratively work on.

[Link to repo](https://github.com/Bosch-0/Bitcoin-Icons)



## 📙 Contributing to Bitcoin Design Guide
Project Muggle will be contributing what we learn through working on Bitcoin Core to the open source [Bitcoin Design Guide](https://github.com/BitcoinDesign/Guide). Learnings obtained through working on Bitcoin Core will likely make valuable additions to the "Open source & open design" section of the Guide.

> The Bitcoin Design Guide is a free open-source community resource that helps designers, developers and others working on non-custodial bitcoin-products to create better experiences, faster. We hope that, over time, it will cover all relevant types of products, including consumer wallets, merchant interactions, exchanges and more. Better products and experiences should ultimately make it more appealing for anyone to own and use bitcoin.



## ☎️ Bi-weekly Bitcoin Core Design Review Calls
Project Muggle along with the Bitcoin Design community hosts bi-weekly Bitcoin Core design review calls. The goal of these calls is to bridge the designer and developer gap and keep the design community up to date with whats going on design and development wise on Bitcoin Core, including work Project Muggle is doing. Scheduled calls can be found in the issues section in the [BitcoinDesign/Meta repo](https://github.com/BitcoinDesign).



## 🛠️ Bitcoin Core GUI pull request (PR) testing
A major development bottleneck for the Bitcoin Core project is the limited amount of PR testers. This issue is amplified with the GUI which needs to be manually tested accross various operating systems. Additionaly, Bitcoin Core has few design focused testers / contributors resulting in the design of many PRs mostly being an afterthought or unfounded in design principlies. 

To assist with bridging the designer / developer gap, Project Muggle will be actively testing GUI PRs. Learnings gained through testing PRs will be valuable in establishing design procedures for Bitcoin Core, as well as be useful for the wider Bitcoin community (such as contributing to the Bitcoin Design Guide). 

Project Muggle will also be aiming to encourage more users (designers or not) to start testing PRs with well designed guides and documentation (see guides and documentation sections below).



## 🔬 Research
Project Muggle conduct design research on how to best implement UI/UX features of the novel constraints that Bitcoin Core has on its products.

Project Muggle will actively collaborate with Bitcoin Core wallet research project [Project Horizon](https://docs.google.com/document/d/1Z2D1Wn5tkQ-Scdp0n8qm2mnFvik1wnU3vcu1DZ1f9jo/edit#) were relevant. Project Muggle will also be implementing / contributing to the Bitcoin Design guide throughout its research.

<details>
  <summary>Research areas of interest</summary>
  
- Designing for Bitcoin Core post 0.21.0 – Taproot, MuSig, descriptors and more.
- UX friendly wallet backups without BIP39.
- Multisig integration with hardened hierarchical Deterministic Wallets.
- Bitcoin Core hardware wallet integration.
- Node bootstrapping.

</details>



## 🖥️ GUI Designs
project Muggle will be actively working on improving the UI/UX of the Bitcoin Core graphical user interface (GUI). Design scope will focus on changes that will be atomic (versioned), non-contentious and translatable to future frameworks such as QML (to not incur design debt). Contributing designs will also assist with establishing design workflows and processes that intergrate with the current Bitcoin Core contributing guidelines. 

Some designs may be prototyped in other open source Bitcoin Projects that have a faster developmental pace than Bitcoin Core. These projects will be labelled as segeu designs.  


### QML GUI
Project Muggle will be working on a complete new QML based design for the GUI. QML offers much more design flexibility than the currently used Qt widgets framework. Switching the Qt framework to QML from widgets is still a [WIP](https://github.com/bitcoin/bitcoin/pull/16883), though designs will be worked on while this transition occurs.

Project Muggle will be applying a minimilist monochrome styling for this design which aligns with the neutral and conservative nature of the Bitcoin Core project.

**More details coming soon.**


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

<details>
   <summary> Version 0.1 </summary>

Version 0.1 focuses on re-working of the current content. This is to make it more clear to users about what they actions they are taking / trade offs they are making. This version has been shared on GitHub for feedback [issue #77](https://github.com/bitcoin-core/gui/issues/77#issue-687141626). [Link]()to active design work. 

</details>
 
<details>
   <summary> Version 0.2 </summary>
  
Version 0.2 focuses on adding extra features to the basic create wallet flow. Examples include HWW integration and descriptor imports. [Link]()to active design work.
  
</details>
 

### CoinControl


[Some great discussions](https://github.com/BitcoinDesign/Guide/issues/22) and work is happening over at the Bitcoin Design community on improving CoinControl UX. Will be implementing these insights from here into the GUI's current coin control UI/UX.


### Hardware wallet intergration
This will likely occur in parallel to v2.0 of the create wallet designs which integrates HWW UI when creating a wallet. This will include things like signing tx's within the GUI using a hardware wallet.  


### Multisig 
Once the GUI has a basic HWW create wallet flow UI implemented, multisig UI is the next priority. Multisig in Bitcoin Core is quite different from other wallets (due to no BIP39 implementation) so this will need to be designed from the ground up. 


### Descriptor wallets
Descriptor wallets included in the next major Bitcoin Core release (0.21) offer a wide range of UX implications. There does not yet exist any reference UI/UX best practices for working with descriptors so this project will be working on building. Some examples of UX improvements descriptors can offer are below:

- Easier multisig backups.
- Better wallet management. 
 


## 📄 Documentation
Project Muggle will create documentation as part of developing design foundations for Bitcoin Core.

<details>
 <summary>List of Documentation</summary>

- **WIP** [design_process.md](https://github.com/Bosch-0/Project-Muggle/blob/master/docs/design_process.md) for how to contribute designs to Bitcoin Core.
- **WIP** [icon_policy.md](https://github.com/Bosch-0/Project-Muggle/blob/master/docs/icon_policy.md) on how to contribute icons to Bitcoin Core. 
- **WIP** Design issue template for bitcoin-core/gui. 

</details>



## 🗺️ Guides
Project Muggle will create simple how-to guides to help end users navigate products developed by Bitcoin Core. Guides will be published on Medium / GitHub and my personal site (coming soon).

<details>
 <summary>List of guides</summary>

 - Compiling Bitcoin Core GUI from source for designers. [Windows](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-windowsos-1e73f478a799), [macOS](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-macos-7ef2e1c6d8b0), [Linux](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-linux-936ed2fca125)
 - **WIP** Setting up your Bitcoin Core GUI node.
 - **WIP** Generating a multisig wallet on the Bitcoin Core GUI.
 - **WIP** Connecting you Bitcoin Core GUI node over Tor.
 
</details>



## 🗯️ Design discussions
Project Muggle aims to actively keep design focused dialogues going between the Bitcoin Core community, developers and designers. 

<details>
  <summary>List of discussions</summary>

- [Bitcoin Core Branding](https://github.com/bitcoin-core/gui/issues/89).
- [Bitcoin Core / Research the history of Core GUI changes through Github issues](https://github.com/BitcoinDesign/Meta/issues/19) 
- Switching net's within the gui [issue #78](https://github.com/bitcoin-core/gui/issues/78)
- Establishing Bitcoin Core design system. 
- Switching Qt framework from widgets to QML.
- Headless Bitcoin Core GUI.

</details>



## 🤏 Minor design contributions
<details>
  <summary>Below are minor UI/UX contributions Project Muggle has made</summary>
 
- Add Tor icon to GUI [issue #58](https://github.com/bitcoin-core/gui/issues/58) / [PR #86](https://github.com/bitcoin-core/gui/pull/86)
- Slight GUI UI/UX improvement when creating wallets [PR #96](https://github.com/bitcoin-core/gui/pull/96)
- Privacy mode toggle option [issue #82](https://github.com/bitcoin-core/gui/issues/82)
- More informative tray icons [issue #70](https://github.com/bitcoin-core/gui/issues/70)
- **WIP** Polish current GUI icon set. [Link](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Website-Design-System?node-id=1881%3A6) to active design work. 

 </details
