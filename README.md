<p align="center">
	<a href="https://github.com/ThaUnknown/miru">
		<img src="./web/static/logo_filled.svg" width="200">
	</a>
</p>
<h1 align="center"><b>Miru</b></h1>

<h4 align="center"><b>Stream anime torrents, real-time with no waiting for downloads</b></h4>

<p align="center">
  <a href="https://miru.watch/#about">About</a> •
  <a href="https://miru.watch/features/">Features</a> •
  <a href="https://miru.watch/faq/">Frequently Asked Questions</a> •
  <a href="#building-and-development">Building and Development</a> •
  <a href="https://miru.watch/download/">Download</a>
</p>
<p align="center">
  <img src="./docs/out.gif" alt="showcase"><br>
  <a href="https://discord.gg/Z87Nh7c4Ac">
    <img src="https://img.shields.io/discord/953341991134064651?style=flat-square" alt="chat">
  </a>
  <a href="https://miru.watch/download/">
    <img alt="GitHub all releases" src="https://img.shields.io/github/downloads/ThaUnknown/miru/total?style=flat-square">
  </a>
</p>

## **About**
A pure JS BitTorrent streaming environment, with a built-in list manager. Imagine qBit + Taiga + MPV, all in a single package, but streamed real-time. Completly ad free with no tracking/data collection.

This app is meant to feel look, work and perform like a streaming website/app, while providing all the advantages of torrenting, like file downloads, higher download speeds, better video quality and quicker releases.

Unlike qBit's sequential, seeking into undownloaded data will prioritise downloading that data, instead of flat out closing MPV.
## **Features**
### **Anime:**
- full AniList integration
  - filter anime by name, genre, season, year, format, status
  - view anime on your planning and watching list
  - add and remove anime from your planning list
  - automatically mark episodes as complete as you watch them
  - view trailers/previews for anime
  - score anime
  - view anime relations
- automatically find torrents for desired episodes
- automatically detect what anime a torrent is
- view latest releases on any custom RSS
- airing schedule
- find anime by image [just paste an image into the app]
### **Video:**
- full subtitle support
  - support for softcoded subtitles
  - support for external subtitle files
  - support for VTT, SSA, ASS, SUB, TXT subtitles
  - subtitle display in PiP
- keybinds for all functions:
  - **S** - seek forwards 90 seconds [skip opening]
  - **R** - seek backwards 90 seconds
  - **→** - seek forwards 2 seconds
  - **←** - seek backwards 2 seconds
  - **↑** - increase volume
  - **↓** - decrease volume
  - **M** - mute volume
  - **C** - cycle through subtitle tracks
  - **N** - play next episode [if available]
  - **B** - play last episode [if available]
  - **F** - toggle fullscreen
  - **P** - toggle picture in picture
  - **[** - increase playback speed
  - **]** - decrease playback speed
  - **\\** - reset playback speed to 1
  - **I** - view video stats for nerds
  - **`** - open keybinds UI
- editable keybinds **`** allows drag dropping any key
- miniplayer
- media session display
- media keys support
- Discord rich pressence
- preview thumbnails
- pause on lost focus
- autoplay next episode
- multi-audio support
- torrent download progress on the seek bar
### **Torrent:**
- select downloads folder
- specify download/upload speeds
- support for most popular BEP's
- support for custom torrent RSS feeds for latest releases
- change what resolution to find torrents in
- stream real-time with no waiting for downloads
- support for custom extensions for custom sources and trackers

## **Installing on Linux**

### Universal (Flatpak)
- Follow the steps [here](https://flathub.org/setup) to set up flatpak and flathub if you haven't already.
- Install [Miru](https://flathub.org/apps/io.github.thaunknown.miru) from a graphical app store or the command line:
```bash
flatpak install io.github.thaunknown.miru
```

### Universal (AppImage)
- Download `linux-Miru-version.AppImage` from the [releases](https://github.com/ThaUnknown/miru/releases/latest) page.
- Run it either directly or with your favorite AppImage manager, such as [GearLever](https://github.com/mijorus/gearlever).

### Arch
- Use your favorite AUR manager to download `miru-bin`. For example:
```bash
paru -S miru-bin
```

### Debian/Ubuntu
- Download `linux-Miru-version.deb` from the [releases](https://github.com/ThaUnknown/miru/releases/latest) page.
- Install the deb file with package manager.
```bash
apt install ./linux-Miru-*.deb
```

### Fedora and its derivatives
- Download `linux-Miru-version.rpm` from the [releases](https://github.com/ThaUnknown/miru/releases/latest) page.
- Install the rpm file with package manager.
```bash
dnf install ./linux-Miru-*.rpm
```

## **Building and Development**

### Electron version
Dependencies:
 - Node 16 or above
 - PNPM

```bash
git clone https://github.com/ThaUnknown/miru
cd miru/electron
pnpm install
pnpm run build
```

---
### Capacitor (Android) version
*good luck*

Dependencies:
 - Node 16 or above
 - PNPM
 - Docker
 - Android Debug Bridge
 - Java 18 or above [probably?]
 - maybe others... have fun.