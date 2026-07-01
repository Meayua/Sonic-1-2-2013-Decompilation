A Full Decompilation of Sonic 1 & 2 (2013). Ported to the Switch.

# **SUPPORT THE OFFICIAL RELEASE OF SONIC 1 & 2**
+ Without assets from the official releases, this decompilation will not run.

+ You can get official releases of Sonic 1 & Sonic 2 from:
  * Windows
    * Via Steam, from [Sonic Origins](https://store.steampowered.com/app/1794960)
    * Via the Epic Games Store, from [Sonic Origins](https://store.epicgames.com/en-US/p/sonic-origins)
  * Nintendo Switch, from [Sonic Origins on the eShop](https://www.nintendo.com/games/detail/sonic-origins-switch/)
  * iOS, Via the App Store
  * Android, Via Google Play or Amazon
    * Note that the mobile releases have been delisted. However, if you have downloaded one of these releases in the past, you can redownload it at any time in your device or store account's purchase history.

Even if your platform isn't supported by the official releases, you **must** buy or officially download it for the assets (you don't need to run the official release, you just need the game assets). See [here](https://rsdkmodding.com/Guides/Games/Sonic1-2/Datapack/) for a guide on how to find the required assets from your legally obtained copy/copies of the game(s).

If you want to transfer your save from the official mobile versions, the **Android pre-forever** file path is `Android/data/com.sega.sonic1 or 2/SGame.bin` (other versions may have different file paths). Copy that file to the `SData.bin` in the EXE folder.

## Installation Instructions
You can find downloads in [releases](https://github.com/Meayua/Sonic-1-2-2013-Decompilation/releases).

1. Make sure your Switch can [run homebrew](https://switch.hacks.guide).
2. Extract the contents of the zip to the root of your SD card.
3. Copy Data.rsdk to `/switch/s12013` or `/switch/s22013` on your Switch's SD card. You can get it from the "assets" folder of the APK. (Which you can open using 7-zip.)
    - If you find "Data.rsdk.xmf" instead, just rename it to "Data.rsdk".
4. Start Sonic 1/2 via hbmenu (or whatever method you prefer).

NOTE: It is recommended to give the game full RAM access. This means you shouldn't launch hbmenu from the album applet when running this. With the latest Atmosphere build and its default config, you can hold R while starting any game to open hbmenu with full RAM access. If you have any issues make sure the game has full RAM access before reporting them; launching as an applet will not be supported.

# How to build

## Switch
1. Acquire [DevKitPro](https://devkitpro.org/wiki/Getting_Started)
2. Install `switch-zlib switch-sdl2_mixer switch-sdl2 switch-pkg-config switch-opusfile switch-mpg123 switch-mesa switch-libvorbisidec switch-libtheora switch-libpng switch-libopus switch-libogg switch-libmodplug switch-libdrm_nouveau switch-glad switch-flac switch-cmake switch-dev` (yes I copied what I had installed.)
3. Clone the repo **recursively**, using: `git clone --recursive https://github.com/RSDKModding/RSDKv4-Decompilation` (If you've already cloned the repo, run this command inside of the repository: ```git submodule update --init --recursive```)
4. Simply run `make`, and pray, ***hard***.

Results will be in bin/switch

# FAQ

### Q: I found a bug!
A: No. The repository is archived. All I've done is re-compile it to support the latest ABI. If you'd like to fix it though, check if it occurs on [here first](https://github.com/RSDKModding/RSDKv4-Decompilation), then go bother them. The issues are closed for a reason.

## Below is the unchanged ending of the readme

# Special Thanks
* [Lulu](https://github.com/MGRich) for helping me fix bugs, tweaking up my sometimes sloppy code and generally being really helpful and fun to work with on this project
* The Weigman for creating the header you see up here along with similar assets
* Everyone in the [Retro Engine Modding Server](https://dc.railgun.works/retroengine) for being supportive of me and for giving me a place to show off these things that I've found

# Contact:
Join the [Retro Engine Modding Discord Server](https://dc.railgun.works/retroengine) for any extra questions you may need to know about the decompilation or modding it.
 
