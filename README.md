![banner image](https://github.com/Bosch-0/Project-Muggle/blob/master/assets/images/bannerimage.png "Banner Image")

# 🧙‍ What is Project Muggle? 
Project Muggle is an initiative started in the [Bitcoin Design community](https://github.com/BitcoinDesign) to improve the design focus of applications developed by the [Bitcoin Core project](https://bitcoincore.org/). The Bitcoin Core project maintains and releases an open source Bitcoin client called “[Bitcoin Core](https://github.com/bitcoin).” Bitcoin Core is (currently) the primary reference implementation for the digital currency Bitcoin (BTC).  

Bitcoin has yet to break out of the non-magical community (programming wizards) into the world of ordinary human beings (muggles). Design is one way to help bridge this gap and make the magical internet money known as bitcoin more accessible to the average person.

This repo will keep track of efforts made in improving the design focus of Bitcoin Core. If you wish to collaborate on Project Muggle reach out on the [Bitcoin Design Slack](https://bitcoindesign.slack.com/join/shared_invite/zt-gytq2snl-4TEWJOTKrXRCB4YLBoDunA#/) or [twitter](https://twitter.com/_bosch_). 



# 🏆 Goal of Project Muggle 
Establish design foundations and direction for Bitcoin Core. 


### What will this achieve?

- Better UI/UX for current and future users of Bitcoin Core products such as the GUI. 
- More design focused contributors / stronger design contribution process within Bitcoin Core.
- Save time and resources by reducing developmental debt - both technical and design.
- Assist with establishing Bitcoin open design processes and standards that help the wider Bitcoin ecosystem. 



# Primary Focuses Timeline
## 🌌 [#1 Establish a Bitcoin Core Design system](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Bitcoin-Core-Design-System?node-id=1830%3A608)
Currently no design system exists within the Bitcoin Core project. Project Muggle will establish a Figma based design system for Bitcoin Core that can be used in its products such as the GUI as well as their website. This will also include some minor re-branding which is [currently underway](https://github.com/bitcoin-core/gui/pull/199). 

- A single, full fledged design system including design and code snippets will eventually be hosted on GitHub pages through a live, interactive web app.



## 🌐 [#2 Redesign Bitcoincore.org](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Bitcoin-Core-Design-System?node-id=2280%3A0)
Project Muggle will be working on a re-design of bitcoincore.org using our Bitcoin Core design system. 

[Bitcoincore.org](https://bitcoincore.org/) currently has a dated and not so user friendly design. User journey's do not start with running an application. In the case of the GUI downloading the binaries from a trusted source such as bitcoincore.org is a first step. The current design does not communicate trust nor does it do a good job educating users about Bitcoin Core and what it offers. A re-design that puts emphasis on user experience and trust will significantly improve how users view Bitcoin Core and its associated products.



## 🖥️ [#3 Redesign a QML based GUI](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Bitcoin-Core-Design-System?node-id=2280%3A110)
Project Muggle will be actively working on improving the UI/UX of the Bitcoin Core graphical user interface (GUI) whilst applying the Bitcoin Core design system. Design scope will focus on changes that will be atomic (versioned), and non-contentious.



# Secondary Focuses
## 📙 Contributing to Bitcoin Design Guide
Project Muggle will be contributing what we learn through working on Bitcoin Core to the open source [Bitcoin Design Guide](https://github.com/BitcoinDesign/Guide). Learnings obtained through working on Bitcoin Core will likely make valuable additions to the "Open source & open design" section of the Guide among others.

> The Bitcoin Design Guide is a free open-source community resource that helps designers, developers and others working on non-custodial bitcoin-products to create better experiences, faster. We hope that, over time, it will cover all relevant types of products, including consumer wallets, merchant interactions, exchanges and more. Better products and experiences should ultimately make it more appealing for anyone to own and use bitcoin.



## 🟠 [Open source Bitcoin icon library](https://github.com/Bosch-0/Bitcoin-Icons)
Project Muggle will be developing an open source bitcoin centric icon library that projects like Bitcoin Core can use in their applications. This will be an open initiative that Project Muggle and the wider Bitcoin Design community will collaboratively work on.



## 🛠️ Bitcoin Core GUI pull request (PR) testing
A major development bottleneck for the Bitcoin Core project is the limited amount of PR testers. This issue is amplified with the GUI which needs to be manually tested across various operating systems. Additionally, Bitcoin Core has few design focused testers / contributors resulting in design direction of many PRs mostly being an afterthought or unfounded in design principles. 

To assist with bridging the designer / developer gap, Project Muggle will be actively testing GUI PRs. Learning's gained through testing PRs will be valuable in establishing design procedures for Bitcoin Core, as well as be useful for the wider Bitcoin community (such as contributing to the Bitcoin Design Guide). 

Project Muggle will also be aiming to encourage more users (designers or not) to start testing PRs with well designed guides and documentation (see guides and documentation sections below).



## 🔬 Research
Project Muggle conduct design research on how to best implement UI/UX features within the novel constraints Bitcoin Core products such as the GUI has. 

<details>
  <summary>Research areas of interest</summary>
  
- Designing for Bitcoin Core post 0.21.0 – Taproot, MuSig, descriptors and more.
- UX friendly wallet backups without BIP39.
- Multisig integration with hardened hierarchical Deterministic Wallets.
- Bitcoin Core hardware wallet integration.
- Node bootstrapping.
- Who is the GUI being designed for? 

</details>



## ☎️ Bi-weekly Bitcoin Core Design Review Calls
Project Muggle, along with the Bitcoin Design community, hosts bi-weekly Bitcoin Core design review calls. The goal of these calls is to bridge the designer and developer gap and keep the design community up to date with whats going on design and development wise on Bitcoin Core, including work Project Muggle is doing. Scheduled calls can be found in the issues section in the [BitcoinDesign/Meta repo](https://github.com/BitcoinDesign).



## 📄 Documentation
Project Muggle will create documentation as part of developing design foundations and processes for Bitcoin Core.

<details>
 <summary>List of Documentation</summary>

- **WIP** [design_process.md](https://github.com/Bosch-0/Project-Muggle/blob/master/docs/design_process.md) for how to contribute designs to Bitcoin Core.
- **WIP** [icon_policy.md](https://github.com/Bosch-0/Project-Muggle/blob/master/docs/icon_policy.md) on how to contribute icons to Bitcoin Core. 
- **WIP** Design issue template for bitcoin-core/gui. 

</details>



## 🗺️ Guides
Project Muggle will create simple how-to guides to help end users navigate products developed by Bitcoin Core. Guides will be published on Medium / GitHub. 

<details>
 <summary>List of guides</summary>

 - Compiling Bitcoin Core GUI from source for designers. [Windows](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-windowsos-1e73f478a799), [macOS](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-macos-7ef2e1c6d8b0), [Linux](https://medium.com/@_Bosch_/compiling-the-bitcoin-core-gui-from-source-for-designers-linux-936ed2fca125)
 - **WIP** Setting up your Bitcoin Core GUI node.
 - **WIP** Generating a multisig wallet on the Bitcoin Core GUI.
 - **WIP** Connecting you Bitcoin Core GUI node over Tor.
 - **WIP** Backing up your Bitcoin Core private keys. 
 
</details>



## 🗯️ Design discussions
Project Muggle aims to actively keep design focused dialogues going between the Bitcoin Core community, developers and designers. 

<details>
  <summary>List of discussions</summary>

- [Bitcoin Core Branding](https://github.com/bitcoin-core/gui/issues/89).
- [Research the history of Core GUI changes through Github issues](https://github.com/BitcoinDesign/Meta/issues/19) 
- Switching net's within the GUI [issue #78](https://github.com/bitcoin-core/gui/issues/78)
- Establishing Bitcoin Core design system. 
- Switching Qt framework from widgets to QML.
- Headless Bitcoin Core GUI - are desktop nodes the way forward?
- Encrypting Bitcoin Core wallet's meta content, not just private keys. 

</details>



## 🤏 Minor design contributions
<details>
  <summary>Below are minor UI/UX contributions Project Muggle has made:</summary>
 
- Add Tor icon to GUI [issue #58](https://github.com/bitcoin-core/gui/issues/58) / [PR #86](https://github.com/bitcoin-core/gui/pull/86)
- Slight GUI UI/UX improvement when creating wallets [PR #96](https://github.com/bitcoin-core/gui/pull/96)
- Privacy mode toggle option [issue #82](https://github.com/bitcoin-core/gui/issues/82)
- More informative tray icons [issue #70](https://github.com/bitcoin-core/gui/issues/70)
- **WIP** Polish current GUI icon set. [Link](https://www.figma.com/file/0oqnohjahRtprjRyaetDOL/Website-Design-System?node-id=1881%3A6) to active design work. 

 </details
