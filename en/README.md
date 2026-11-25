# Download OtoWake BG

[日本語](../ja/README.md)

**The current version is 0.1.0 (beta).** It is a first version with a reduced set of features, released to gather feedback and bug reports before the final version. How it works and looks may still change.

OtoWake BG is a free practice app for people who play bluegrass. It takes the song that is playing and plays it again split into parts: vocals, banjo, mandolin, fiddle, dobro, guitar, bass and more. Turn down the part you want to play, and the recording becomes your backing band.

What it can do, and what to know before you use it, is in the [Release Notes](release-notes.md). How to use it is in the [Mac guide](manual-mac.md) and the [Windows guide](manual-windows.md) (both also open from the app's Help).

## Download

| | File | Size | Runs on |
|---|---|---|---|
| Mac | [OtoWakeBG-0.1.0-mac.pkg](https://github.com/OtoWakeBG/otowake-bg/releases/download/v0.1.0/OtoWakeBG-0.1.0-mac.pkg) | 143 MB | A Mac with Apple silicon, macOS 14.2 or later |
| Windows | [OtoWakeBG-Setup-0.1.0-win-x64.exe](https://github.com/OtoWakeBG/otowake-bg/releases/download/v0.1.0/OtoWakeBG-Setup-0.1.0-win-x64.exe) | 187 MB | Windows 11 (x64); a DirectX 12 GPU is recommended |

It does not run on Intel Macs, Windows 10 or Windows on ARM.

The installer speaks English or Japanese, following your computer's language. You can change the app's language later in its settings.

## First: you will see a warning, and that is expected

> [!CAUTION]
> **The OtoWake BG installers and app carry no developer signature from Apple or Microsoft,** because it is made by an individual and given away for free. When you download it or open it for the first time, your Mac or PC warns that it cannot verify it. The steps below get you past the warning.
>
> - **On Windows, it cannot run on a PC where "Smart App Control" is on** (see "It does not run with Smart App Control on" below).
> - If you want to be sure, check that the file is the one we published before you open it (see "Check the file" on this page).

## Install on a Mac

1. Download `OtoWakeBG-0.1.0-mac.pkg` and double-click it.
2. If you see “OtoWakeBG-0.1.0-mac.pkg” Not Opened, press "Done" (not "Move to Trash").
3. Open System Settings from the Apple menu and choose "Privacy & Security".
4. Under "Security" near the bottom, it says “OtoWakeBG-0.1.0-mac.pkg” was blocked to protect your Mac. Press "Open Anyway" next to it.
5. When asked again, press "Open Anyway" and confirm with your login password (or Touch ID).
6. The installer opens. Go through it with "Continue", then press "Install".
   - Under "Destination", "Install for me only" puts the app in the Applications folder of your home folder, without an administrator password.
7. When it is done, open OtoWake BG from the Applications folder. An icon appears in the menu bar.

On macOS 14, instead of steps 2–5, Control-click the `.pkg` and choose "Open".

If the same warning appears when you open the app, press "Open Anyway" in the same way (steps 3–5).

## Install on Windows

1. Download `OtoWakeBG-Setup-0.1.0-win-x64.exe`.
   - If Microsoft Edge says it "isn't commonly downloaded", choose "Keep" from the "…" on that line, then "Show more" → "Keep anyway".
2. Double-click the downloaded file.
3. If you see "Windows protected your PC", press "More info", then "Run anyway".
4. In the setup, choose whether to create a desktop shortcut, then press "Next", "Install" and "Finish". You need no administrator rights.
5. OtoWake BG starts. You can also start it from "OtoWake BG" in the Start menu.

### It does not run with Smart App Control on

> [!CAUTION]
> **On a PC where Windows 11's "Smart App Control" is on, apps without a signature are blocked and OtoWake BG cannot run.** Unlike the warnings, there is no way past this.

To check: open "Windows Security" from the Start menu, then "App & browser control" → "Smart App Control settings". If it says "On", this version cannot be used.

Once Smart App Control is turned off, it cannot be turned back on without reinstalling Windows. We do not recommend turning it off for OtoWake BG.

## Check the file (SHA-256)

You can check that the file you downloaded is the one we published. If the value below matches the one your computer calculates, the file has not been changed on the way.

| File | SHA-256 |
|---|---|
| `OtoWakeBG-0.1.0-mac.pkg` | `264fb6b7ba328f8bac5325b76d21a9d9eadaabe98596788afaa05f7b2af8a65d` |
| `OtoWakeBG-Setup-0.1.0-win-x64.exe` | `efbd9b48cb6dedb2e688709aafa872d38e02bf1679f0cc04166e24463c176d41` |

- Mac: in Terminal, type `shasum -a 256 ` (with one space at the end), drag the downloaded file onto the window, and press Return.
- Windows: right-click in the download folder, choose "Open in Terminal", type `certutil -hashfile OtoWakeBG-Setup-0.1.0-win-x64.exe SHA256` and press Enter.

## Uninstall

- Mac: quit OtoWake BG, then move OtoWake BG from the Applications folder to the Trash. To remove your settings and data too, move `~/Library/Application Support/OtoWake BG` to the Trash as well.
- Windows: use "Uninstall OtoWake BG" in the "OtoWake BG" Start menu folder, or Settings → Apps → Installed apps. Your settings and data (`%APPDATA%\OtoWake BG` and `%LOCALAPPDATA%\OtoWake BG`) are kept.

## Please

- Use only audio you are allowed to use. Whether you may capture or process audio depends on the rights in the recording and on the terms of the service that plays it. See "Things to know before you use it" in the [Release Notes](release-notes.md).
- The split is not perfect. Listen and check as you go.

## Credits and contact

The credits for the technology and material it uses are in [Credits](../credits.md).

Send bug reports and feedback by direct message, to either of these. We do not take feedback by email.

- X: a direct message to [@OtoWakeBG](https://x.com/OtoWakeBG)
- Substack: a direct message to [OtoWake BG](https://otowakebg.substack.com)

When you report a problem, it helps to include your OS and version, your Mac model or your PC's CPU and GPU, and what you did and what happened.
