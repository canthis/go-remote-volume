# ![Go Remote Volume ](https://dev.canthis.lv/storage/app/media/Screenshots/goremote-icon-32x32.png) Go Remote Volume 
![GitHub release](https://img.shields.io/github/release/canthis/go-remote.svg?label=version)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/canthis/go-remote-volume/blob/master/LICENSE)

Basic app written in golang and Vue.js to Shutdown PC and control master volume over LAN/WiFi (Currently Windows only)

- Golang is used for backend (expose API endpoints and change volume).
- Vue.js is used to provide WEB interface and interact with backend API.

## Build
```
go generate
go build -ldflags -H="windowsgui -s -w" -o "GoRemote.exe"
rice append /exec "GoRemote.exe"
```
This should compile ```GoRemote.exe``` file

## Running
- Download: [GoRemote-amd64.exe (64-bit)](https://github.com/canthis/go-remote/releases/latest/download/GoRemote-amd64.exe) 
or [GoRemote-i386.exe (32-bit)](https://github.com/canthis/go-remote/releases/latest/download/GoRemote-i386.exe)
- Launch it and navigate from you mobile browser to your PC's Local IP, e.g. ```localhost:8775``` or ```192.168.x.x:8775```
- Add it Home Screen and enjoy


## Screenshot
<p>
<img src="https://dev.canthis.lv/storage/app/media/Screenshots/go-remote-volume-chrome-android-v0330.png" width="25%" height="25%" />
</p>

## Credits
- https://github.com/itchyny/volume-go
- https://github.com/GeertJohan/go.rice
- https://github.com/josephspurrier/goversioninfo
- https://github.com/gen2brain/beeep
- https://github.com/getlantern/systray
- https://github.com/julienschmidt/httprouter
- https://codepen.io/calebbrewer/pen/pdyNbb
- App Icon made by [Smashicons](https://www.flaticon.com/authors/smashicons) from [www.flaticon.com](https://www.flaticon.com/) is licensed by [CC 3.0 BY](http://creativecommons.org/licenses/by/3.0/)


## License
This software is released under the MIT License, see LICENSE.

