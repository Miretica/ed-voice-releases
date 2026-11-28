<img src="icon.png" alt="ED Voice" width="96" align="right">

# ED Voice

**Hear your Elite Dangerous comms, and know when you're in danger.** ED Voice reads the game's chat aloud while you fly: messages from other commanders, your wing and squadron, stations and NPCs, each with their own voice. It sounds the alarm when a ship turns hostile, and your ship's computer talks to you about jumps, the systems you arrive in, and its own condition. The voices run **locally on your PC**, so it works offline and nothing is sent anywhere.

### ⬇️ [Download the latest version](https://github.com/Miretica/ed-voice-releases/releases/latest)

Download `EdVoiceApp-win-Setup.exe` from the latest release and run it.

---

## Features

### Chat, read aloud
- 🗣️ **Natural-sounding voices** (Kokoro) that run on your own computer: no cloud, no account.
- 🎭 **A voice for every commander.** Commanders you chat with directly, or in wing and squadron chat, join your **Commanders** list and keep their own voice. Their messages go first, with a short radio tone, while other chat fades down.
- 🛰️ **NPCs in five groups** (stations, system, military, civilians, criminals), each pilot with a voice of its own. Repeated phrases such as "Docking request granted." play instantly.
- 😄 **Understands chat:** `o7`, `CMDR`, numbers, times, contractions and emoticons (`:D` → "ha ha"). Danish and Norwegian messages are read with matching sounds.

### Threats and scans
- 🚨 **Red alert** when a ship turns hostile: a pirate scanning your cargo or demanding it, a hunter that found you, an interdiction (announced the moment it starts), an attack, your shields going down. Your ship tells you who it is and what they're doing, before anything else is spoken.
- ⚠️ **Yellow alert** for possible threats, such as a Powerplay agent that spotted you.
- 📋 **Threats and Scans panels**: every ship that is, or may be, hostile, with its ship, rank, legal status and bounty once you target it, and who scanned you. Rival Powerplay ships are recognised even when they're "Clean".

### Your ship's computer
- 👋 Greets you, announces **jumps** (with fuel-scooping and dangerous-star hints) and **reports each system** you arrive in: security, Power, state, conflicts and what to watch out for.
- 🛡️ Reports its **condition**: *"Shields down!"*, overheating, *"Reboot complete"*, low fuel, and the threat level of signal sources you drop into.
- 🧭 A cockpit-style **status bar**: your commander, ship, balance, system, Power and notoriety.

### The chat view
- 💬 **Message cards in Elite style**, with a calm feed; warnings and attacks stand out in amber and red.
- ▶️ **Playback on every card:** see whether a message is queued, being generated or speaking, with a progress bar; stop just that message, or play it again.
- 👤 **Add a commander from their message** and pick their voice right there, with a preview and how to pronounce their name.
- 📜 **Scroll up to read older messages** without the feed running away; a pill shows how many new ones came in, and whether any were warnings.
- 🔇 Speech on or off, NPC messages on or off, volume, speed and text size.

## Requirements

- Windows 10 or 11 (64-bit)
- Elite Dangerous on the same PC
- About 400 MB of disk space for the app and the voices

## Install

1. Download **`EdVoiceApp-win-Setup.exe`** from the [latest release](https://github.com/Miretica/ed-voice-releases/releases/latest).
2. Run it. ED Voice installs **for your user account only**, with no administrator rights, and adds shortcuts to the Desktop and Start menu.
   - If the **.NET 10 Desktop Runtime** isn't installed yet, the setup downloads it from Microsoft and installs it first. This step may ask for permission.
3. Start ED Voice and click **Download voices** (about 350 MB, once). Until then the built-in Windows voice is used.
4. Start Elite Dangerous. Messages appear and are read aloud as they arrive.

### "Windows protected your PC"?

ED Voice isn't code-signed yet, so Windows SmartScreen may warn about the installer. Click **More info → Run anyway**. Only download ED Voice from this page.

## Privacy

- ED Voice only **reads** the files that Elite Dangerous writes for third-party tools (the journal and `Status.json` in `Saved Games\Frontier Developments\Elite Dangerous`). It never changes them.
- All speech is generated **on your PC**. Chat messages never leave your computer.
- The app only uses the internet to download the voice model once, from the official [sherpa-onnx release on GitHub](https://github.com/k2-fsa/sherpa-onnx/releases/tag/tts-models). The installer may also download the .NET runtime from Microsoft.

## Uninstall

Windows **Settings → Apps → Installed apps → ED Voice → Uninstall**. This removes the app, the downloaded voices and the cache. Your settings and per-commander voices are kept in `%APPDATA%\EdVoice`; delete that folder too if you want everything gone.

## Known limitations

- The voices are English. Danish and Norwegian messages are pronounced with matching sounds, but with an English accent. Other scripts, such as Cyrillic, aren't read aloud.
- Invented commander names are pronounced from their spelling. Set how a name is pronounced with the person icon on their message, or under **Voices → Spoken as**.
- ED Voice only knows what the game writes to its files. The game doesn't list the ships around you, doesn't report a target's shields and hull as you damage it, and doesn't say who scanned you unless they speak or you target them. So some threats are shown as an *Unknown ship* until they identify themselves.

## Feedback

Found a bug or have an idea? Please open an [issue](https://github.com/Miretica/ed-voice-releases/issues). For problems, include the version (shown under **About**) and what happened.

## License

ED Voice is © 2026 Oleksii Miretskyi, released under the MIT License. It uses third-party components, including sherpa-onnx and the Kokoro-82M voice model (Apache-2.0), NAudio and Velopack (MIT). The full license texts and notices are included in the app under **About**.

*Elite Dangerous is a trademark of Frontier Developments plc. ED Voice is an unofficial, fan-made tool and is not affiliated with or endorsed by Frontier Developments.*
