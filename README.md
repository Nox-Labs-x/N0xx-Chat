<div align="center">
<img src="docs/logo.png" width="72" alt="">

# N0xx Chat

Private chat, voice, video and screen sharing that doesn't eat your PC.

**[Download for Windows](https://github.com/Nox-Labs-x/N0xx-Chat/releases/latest/download/noxx-setup-windows-x64.exe)** ·
[Mac](https://github.com/Nox-Labs-x/N0xx-Chat/releases/latest/download/noxx-macos-arm64.dmg) ·
[Linux](https://github.com/Nox-Labs-x/N0xx-Chat/releases/latest/download/noxx-linux-x64.deb) ·
[All releases](https://github.com/Nox-Labs-x/N0xx-Chat/releases)

<img src="docs/room.png" alt="N0xx Chat room with voice">
</div>

I got tired of chat apps that sit at 500 MB of RAM doing nothing, so I made my own. The installer
is about 3 MB and it idles at basically 0% CPU. A voice call uses around 1%.

It's end-to-end encrypted, there are no accounts, and nothing gets stored anywhere.

### Features

- Text chat (bold, italics, code, links)
- Voice with mute, deafen and per-person volume (right click someone)
- Camera and screen sharing, with optional system audio
- Screen recording straight to your PC
- Rooms use 4-word codes like `orbit maple sugar velvet` instead of long random links

### Installing

**Windows:** run `noxx-setup-windows-x64.exe`. It isn't code-signed yet, so Windows might show
"Windows protected your PC". Click *More info*, then *Run anyway*. No admin needed.

**Mac:** open the .dmg, drag noxx into Applications, then right-click it and pick *Open* the first time.

**Linux:** `sudo apt install ./noxx-linux-x64.deb`. Chat works everywhere. Voice depends on your distro's WebKitGTK having WebRTC.

### Using it

<img src="docs/join.png" width="360" align="right" alt="Joining with a room code">

1. Put in the server link you got from whoever runs your server (something like `https://noxx.tail1234.ts.net`).
   It goes green once it connects.
2. Pick a name.
3. Type a room code a friend sent you, or hit **Create a new room**. Codes don't care about capitals
   or spacing, and the first 4 letters of each word are enough.
4. In a room, **Invite** shows the code and a link. The link has the server in it too, which is
   easier for people who haven't set anything up yet.

Want to host a server for your friends? That's over at
**[N0xx-Chat-server](https://github.com/Nox-Labs-x/N0xx-Chat-server)**. It's one program and you
don't need to port forward.

<br clear="right">

### Privacy

<img src="docs/invite.png" width="400" align="right" alt="Invite window">

The room code is the encryption key. Messages, names and call setup get encrypted (AES-256-GCM)
on your device before anything is sent, and the code itself never leaves your device, so the
server can't read anything. Voice and video go straight between you and your friends.

Anyone with the code can get in, so only send it to people you actually want there.

Full details: [Privacy Policy](PRIVACY.md).

<br clear="right">

---

[Terms](TERMS.md) · [Privacy](PRIVACY.md) · [License](LICENSE) · [Security](SECURITY.md) · [Third-party notices](THIRD-PARTY-NOTICES.md)
