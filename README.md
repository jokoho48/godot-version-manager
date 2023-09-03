<table><tr width=64px><td><img height=64px src="https://user-images.githubusercontent.com/526829/169241046-3087a41d-9606-43ab-90ae-ee0055bef039.png"/></td><td><h1>godot-version-manager</h1></td></tr></table>
  
Download, install and manage any version of Godot Engine from a simple app. 

![image](https://user-images.githubusercontent.com/526829/213944428-2b2d1ffa-8656-4efa-9bf4-dc32f793a6a7.png)

## Installation
### Windows:
Unzip and double-click. Extraction of downloaded versions requires powershell
### Linux:
Unzip and double-click. Extraction of downloaded versions requires `unzip` which, if not installed, should be available in your distro repository
### OSX:
- Should auto extract after download
- You need to run `sudo xattr -r -d com.apple.quarantine path/to/Godot Version Manager.app` since unsigned binaries get marked as untrusted otherwise. Feel free to build the project yourself if you don't trust the prebuilt binaries
- Double click Godot Version Manager.app

## Features
- Automatically download and install any version of Godot from a drop-drown menu. (requires powershell for extraction)
- Show or hide alpha, beta, rc versions from download drop-down. 
- Add your own binaries anywhere on your filesystem. 
- Colorful icons to easily distinguish stable, rc, beta, alpha and master builds. 
- Right click to remove entry entry from the list

## F.A.Q
**Q: Where are the downloaded binaries saved to?**

A: They are saved to `user://versions` which varies depending on your platform. On windows it's %appdata%/Godot/app_serdata/Godot Version Manager/versions

**Q: How is this different from Hourglass or Godot Manager?**

A: [Hourglass](https://hourglass.jwestman.net/) is a much more mature and featureful project which also does project management. Maybe the only advantage GVM has is that it also downloads news snippets from the official website :) [Godot Manager](https://github.com/eumario/godot-manager) seems to be a pretty mature and featureful alternative too. A new (Aug 2023) alternative is [Godots](https://github.com/MakovWait/godots)

**Q: Why do you scrape godotengine.org/news instead or fetching the RSS feed?**

A: The rss doesn't have links to thumbnails or excerpts, only the full text. Also the rss feed contains every entry in the history of Godot News. It's currently a 17MB download.

## TODO
- [x] Linux support
- [x] OSX support
- [ ] Complete refactor
- [ ] Better ~~(i.e some at all)~~ error handling
- [x] Autorefresh, use HEAD for faster scraping, ignore folders without updates.
- [ ] Inform about available updates for installed versions
- [x] Inform about available updates for Godot Version Manager
- [x] Show news snippets from godotengine.com/news?

## LICENSE
MIT Licensed (see LICENSE.md)
Copyright ©️2022 Lisandro Lorea

Lilita One Font ©️2011 Juan Montoreano
<a href="https://www.flaticon.com/free-icons/exe" title="exe icons">Exe icons created by Freepik - Flaticon</a>
