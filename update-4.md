# INTRODUCTION

Welcome to the fourth grant update from Decentraland Alternative Explorer project. This team has the main goal of developing an explorer version using two different technologies:
- Bevy targeting to Desktop
- Godot targeting to Mobile

As secondary objectives we have:
- Make reliable explorer-agnostic tests to ensure the well-working of new explorers
- Develop experimental builds on VR and Web using Godot

The project is progressing as planned.

# HIGHLIGHTS

### General highlights:

Last month we improved a lot the Experience of the Application. We implemented the UI needed for a good experience, and have all your needs there. And also we fixed a lot of bugs, we improved the performance and we polish the components.

### Detailed Godot highlights:

#### Features:
- Custom places generation (#227)
- Audio settings and microphone enablement (#226)
- Discover feature implementation (#211)
- Teleport to spawn point when loading is finished (#221)
- Iterate settings and resolution adjustments (#217)
- OpenSea NFT v2 and multiple image format support for fetching textures (#216)
- Implementation of Archipelago communications (#214)
- Lobby feature introduction (#212)
- Add falling/jump animation (#208)
- UI emotes integration (#238)
- Rounded corners in Discover items (#242)
- Map button with coordinates and SDK6 scene warning (#245)
- Mouse cursor movement on touch on mobile devices (#256)
- Emotes version 2 implementation (#246)
- Profile snapshots upload functionality (#258)
- Trigger scene emote feature (#259)
- Send emote data to scenes and avatar shape fixes (#260)
- Emote wheel editor introduction (#271)
- Requirement to accept terms and privacy policy for new profile deployment (#278)
- Implementation of send and sendBinary over communications (#279)
- Fetch collectibles and remote emotes feature (#292)
- Fetch collectibles wearables from user address (#300)
- Change between first/third person view with zoom in/out on mobile (#303)
- Multiple animation support (#304)
- Profile settings enhancement (#327)
- New theme for Discover, and immediate updates for custom places and last visited visibility (#332)

#### Fixes:
- Fix for main.crdt not loading and visibility component fallback (#223)
- Fix for target position for spawn points (#222)
- Fix for loading issues at start location and empty parcels (#215)
- Full-screen jump in background smoothing and teleportation enhancements (#249)
- After using fallback wearables, eyes/mouth become unchangeable fix (#261)
- Avatar renderer export fix (#262)
- Export resources as tres from unique resources fix (#267)
- Collider attached player issue and other miscellaneous fixes (#269)
- Improvement for teleport to functionality, teleport popup, and backpack avatar preview region (#313)
- Fix for skinned colliders not working properly (#311)
- Websocket support for ArrayBuffer and Array of numbers (#326)
- Profile change flow improvements and initial profile image generation (#290)

#### Refactors:
- Refactor of entity data acquisition and types (#241)

#### Chore:
- Move macOS build to ARM64 architecture (#228)
- Update Rust to version 1.76 (#297)
- Update Goerli-Plaza-IPFS realm (#306)

#### Documentation:
- Minor typo and grammar corrections in README (#309)

You can track the code changed in this month here: https://github.com/decentraland/godot-explorer/compare/d1a3d2b9d14b899b5f4de406fdfe612089496479...32dc9db093c38ae1e02be64a8cb2a4d4c72a0aad

### Detailed Bevy highlights:

#### Features
- UI
- - Built and integrated bevy_dui (data driven ui library)
- - Migrate numerous components to dui (buttons, tabs, combos, text entry, color picker)
- - Add spinner
- - Add dui for login flow
- - Add dui for photobooth
- - Add dui for profile settings
- - Add dui for wearables
- - Add dui for discover page
- - Add dui for map page
- - Add dui for change realm dialog
- - implemented shader for rounded corners / fade border colors
- Map: download and display variable res images, click to teleport
- Minimap
- Load default emotes from remote source
- Add binary message bus, amend string message bus to new format

#### Bugfixes
- Fix tween face direction
- Fix emote urns for owner component
- Support fixedAdapter and adapter comms specs
- Disable colliders for entities parented to player and camera
- Animations now respect should_reset
- Fix sign-message panic when no wallet connected
- Fix emote name alignment
- Fix div by zero for 9slices with no middle
- Fix duplicate settings dialog on spamming button
- Process js::main rpc calls before calling onStart
- Fix h-align for text shapes
- Apply positions to new gltfs after spawn and before rendering for the first time

#### Misc
- Move cache root
- Use released bevy_console
- Add no_fog commands line arg

# Blockers

No blockers in this update.

# Next Steps

As everything seems to be on track as planned, the public roadmap in https://github.com/orgs/decentraland/projects/43 contains what we're working on.

Save the date! We have planned a live test for 19 march for the Mobile version for Android!

March we are going to focus on the stability of the platform, and public to the stores. We're doing QA on the App and fixing bugs.

# Additional notes and links

- Join us on our Discord server: https://discord.com/invite/6mGqPnjujT
- Public home page to get links: https://dclexplorer.com/
- Public roadmap: https://github.com/orgs/decentraland/projects/43
- Godot project: https://github.com/decentraland/godot-explorer/
- Bevy project: https://github.com/decentraland/bevy-explorer/
- Scene Explorer Tests: https://github.com/decentraland/scene-explorer-tests

# Reporting

category,description,token,amount,receiver,link
Team Compensation,(January) Develop and mantain bevy-explorer,DAI,13125,0x85bc980eb632434c562414791146cc86cea12c51,https://etherscan.io/tx/0x0aab99252e6ca89a05c9cdfb05eff29f40123c5fb8454e50ae6b376d6559f3ef
Team Compensation,(January) Develop and mantain godot-explorer,DAI,10500,0x6db12e73904eb12f9c40b7d995b2a870254b3625,https://etherscan.io/tx/0x0aab99252e6ca89a05c9cdfb05eff29f40123c5fb8454e50ae6b376d6559f3ef
Team Compensation,(January) Develop and mantain godot-explorer,DAI,10500,0xbcae59ff0aa916b6c38adde712c39da3eb5443c4,https://etherscan.io/tx/0x0aab99252e6ca89a05c9cdfb05eff29f40123c5fb8454e50ae6b376d6559f3ef
Team Compensation,(January) Develop and mantain scene-explorer-tests,DAI,1200,0xae185e420a7b0e82963f6edb80078d0ce9d40b40,https://etherscan.io/tx/0x0aab99252e6ca89a05c9cdfb05eff29f40123c5fb8454e50ae6b376d6559f3ef
Team Compensation,(January) Team savings,DAI,1041,0xae185e420a7b0e82963f6edb80078d0ce9d40b40,https://etherscan.io/tx/0x0aab99252e6ca89a05c9cdfb05eff29f40123c5fb8454e50ae6b376d6559f3ef