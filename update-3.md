# INTRODUCTION

Welcome to the third grant update from Decentraland Alternative Explorer project. This team has the main goal of developing an explorer version using two different technologies:
- Bevy targeting to Desktop
- Godot targeting to Mobile

As secondary objectives we have:
- Make reliable explorer-agnostic tests to ensure the well-working of new explorers
- Develop experimental builds on VR and Web using Godot

The project is progressing as planned.

# HIGHLIGHTS

### General highlights:

Since last month, both explorers have entered the SDK7 Beta stage. This means that we are still polishing the clients for future beta testing for the users.

The UI was one of the focus this month. Creating menus, improving the interactions with the user, and going to a usable product for everyone.

### Detailed Godot highlights:

#### Performance and Functionality Fixes:
- Reduced export size and resolved issues on mobile and Windows platforms (#129).
- Cleaned imports and bundled empty parcels to streamline operations (#131).
- Addressed various UI issues including text size, canvas size, and texture loading problems (#135).
- Resolved issues with UI tests, NFT classic, and DCL background textures (#136).
- Fixed a bug causing crashes related to content loading (#163).
- Improved response formatting for sendAsync as jsonRPC (#164).
- Addressed content loading-related crashes specifically on Android (#168).
- Fixed a problem where tween wasn't functioning without a TransformComponent in the entity (#171).
-  Solved an issue with UI backgrounds not setting the region rect and not hiding when set to display:none (#195).
- Fixed avatar attach collider and ensured global pointer events send raycast_hit (#199).
- Implemented a hotfix for a wrong skybox instance on mobile.
- Added hidings to the skin category (adr-60) and made wearable URNs ignore tokenId (#179).

#### Refactoring and Improvements:
- Improved content loading process (#132).
- Implemented transparent backgrounds for avatar renderer export images (#160).
- Enhanced performance by deeper throttling for Transform, MeshRenderer, and GltfContainer (#177).

#### New Features:
- Introduced Docker image support (#86).
- Added a feature to build without including ffmpeg, livekit, or deno/v8 in Rust (#170).
- Developed the main HUD for mobile (#169).
- Implemented face_direction and fixed cylinder collider issues (#176).
- Added a new loading screen (#175).
- Introduced a feature to hide the loading screen with a double click on the header (#180).
- Enabled mobile interactions with input actions (#196).

#### Continuous Integration and Documentation:
- Added Godot snapshots and integrated CI for testing with a local server (#165).
- Updated documentation for building Android/Linux with Docker (#174).
- Ran Android builds manually and updated @dcl/scene-explorer-tests (#172, #173).

This summary covers various fixes, refinements, and new features aimed at improving performance, user interface, content loading, and the development process.
You can track the code changed in this month here: https://github.com/decentraland/godot-explorer/compare/11867fd28c2461935b2c69919701f6800aae2662...main

### Detailed Bevy highlights:

#### Features
- Tweens
- Ethereum controller
- Non-default emote support
- PBTextShape refactor and some additional features (no line-spacing, shadows or outlines still)
  - Font
  - Text align
  - Width
  - Padding
  - Line count
- System ui (in progress)
  - Data-driven templates for system ui components
  - Support hot reloading of templates
  - Reworked login / cancel login
  - Emote ui

#### Bugfixes / Infrastructure
- Add js performance api
- Update macos ffmpeg build for ci
- Duplicate hashes in content map caused entries to be ignored

# Blockers

No blockers in this update.

# Next Steps

As everything seems to be on track as planned, the public roadmap in https://github.com/orgs/decentraland/projects/43 contains what we're working on. In February we plan to continue a large bug-fixing stage and start developing the final product, late February we hope to start publishing beta releases and having public beta testing.

# Additional notes and links

- Join us on our Discord server: https://discord.com/invite/6mGqPnjujT
- Public home page to get links: https://dclexplorer.com/
- Public roadmap: https://github.com/orgs/decentraland/projects/43
- Godot project: https://github.com/decentraland/godot-explorer/
- Bevy project: https://github.com/decentraland/bevy-explorer/
- Scene Explorer Tests: https://github.com/decentraland/scene-explorer-tests

# Reporting

category,description,token,amount,receiver,link
Team Compensation,(December) Develop and mantain bevy-explorer,DAI,11812,0x85bc980eb632434c562414791146cc86cea12c51,https://etherscan.io/tx/0x2b4dbd3816b8561f6337d48a8abbab32301f57159a0d2b8e20cc511426257422
Team Compensation,(December) Develop and mantain godot-explorer,DAI,10535,0x6db12e73904eb12f9c40b7d995b2a870254b3625,https://etherscan.io/tx/0x2b4dbd3816b8561f6337d48a8abbab32301f57159a0d2b8e20cc511426257422
Team Compensation,(December) Develop and mantain godot-explorer,DAI,10500,0xbcae59ff0aa916b6c38adde712c39da3eb5443c4,https://etherscan.io/tx/0x2b4dbd3816b8561f6337d48a8abbab32301f57159a0d2b8e20cc511426257422
Team Compensation,(December) Develop and mantain scene-explorer-tests,DAI,1200,0xae185e420a7b0e82963f6edb80078d0ce9d40b40,https://etherscan.io/tx/0x2b4dbd3816b8561f6337d48a8abbab32301f57159a0d2b8e20cc511426257422