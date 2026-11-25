# OtoWake BG — Release Notes

OtoWake BG (read "oh-toh-wah-keh bee-jee") is a practice app for bluegrass players. It takes the song that is playing and splits it into parts, so you can turn each one up or down: vocals, banjo, mandolin, fiddle, dobro, guitar, bass and more.

This is the first limited release, for Mac and Windows: version 0.1.0, a **beta**. It has a reduced set of features and is free to use; how it works and looks may still change before the final version. These notes cover what is in this release, what you should know before you use it, and the credits. Step-by-step instructions are in the manuals: [Mac](manual-mac.md) and [Windows](manual-windows.md).

## 1. What OtoWake BG is

### Who it is for

- Players who want to practise against a real recording, taking the part of one instrument or the vocal.
- Players who want to bring one instrument forward to hear what it is doing.
- Players who need to slow a song down, change its key, or loop a hard passage.
- Anyone who wants to record themselves and hear the take together with the song.

### What it does

You give it audio you are allowed to use: a file, or sound playing on your computer. The app separates it, close to real time, into ten parts:

- vocals, banjo, mandolin, fiddle, dobro, guitar, bass, drums, piano and other

You can change the volume of each part or switch it off. Switch off the part you play, and the recording becomes your backing band.

The model is built for acoustic bluegrass line-ups: voice, banjo, mandolin, fiddle, dobro, guitar and bass.

## 2. What is in this release

- **Separation into parts.** Works on sound playing on your computer and on audio files. Volume, mute and solo for each part.
- **Speed and key.** Play slower without changing the pitch. Change the key in semitone steps, and give the vocals a key of their own if you like.
- **Loops and ranges.** Repeat any passage and save it with a name. The app finds instrumental breaks and sung sections and lists them for you (both are drafts, and the sung sections in particular are rough).
- **Practice tools.** "Hold the current sound" (stop the song and hold the sound that is playing, to find notes and chords by ear), a beat click, a level graph, practice mode (choose your instrument and set the part levels in one go), and practice songs.
- **Key, tempo (BPM) and chords.** Shown as estimates. You can correct them by hand.
- **My recordings.** Record your singing or playing with the microphone and listen to it with the same song.
- **Tablature.** View, edit, play, transpose and export. Photos and PDFs of tab can be read into a draft (support differs between the Mac and Windows editions; see the manuals).
- **Groove Check (experimental).** Measures where each instrument sits in the beat, the rhythm spread, and the pitch of the singing.
- **Transcription with your own AI assistant over MCP (experimental).** Connect your AI assistant to the app and ask it to transcribe a range you have selected. The note candidates are picked from the audio by a simple method, so accuracy is not high.

More features are planned.

## 3. System requirements

### Mac

- macOS 14.2 or later
- A Mac with Apple silicon (Intel Macs are not supported)
- Sound starts a few seconds to over ten seconds after you switch separation on (about 15 seconds for an audio file, which is separated twice and averaged). If your Mac cannot keep up, the app switches by itself to a mode that stores sound before playing it (see "Computer speed and delay" below).

### Windows

- Windows 11 (x64)
- A DirectX 12 graphics card is recommended. The app also runs on the CPU alone, but it may fall behind.

### Both

- Use only audio you are allowed to use (see "Things to know before you use it").
- The experimental AI transcription needs an AI assistant of your own that supports MCP.

## 4. Things to know before you use it

### 4-1. Separation is not perfect

The app estimates each part from the mixed sound with AI. Every part it gives you carries a little of the others.

- **Dobro.** It is separated only to a degree, and its accuracy is still low. Other instruments can end up in the dobro part, and the dobro can end up in other parts.
- **Singing is turned down, not removed.** With the vocals at 0%, a faint voice can still be heard. This is not a clean karaoke or vocal remover.
- **Bass.** Low guitar notes and the voice can show up in the bass part.
- **Banjo.** High guitar notes can land in the banjo part.
- **Guitar.** Mandolin, fiddle and voice can leak into the guitar part.
- **What it is built for.** Acoustic bluegrass line-ups. Songs with drums, piano or electric instruments, and music from other genres, are not handled well.

Results vary a lot from song to song and from recording to recording. Check by ear.

### 4-2. The numbers are estimates

- **Key, BPM and chords** are estimated from the sound and can be wrong. BPM can come out at double or half the real tempo. Chords are limited to major, minor and seventh. Fast chord changes, thin backing and solo passages are where mistakes are most likely.
- **Breaks and sung sections** (the "ranges") are drafts found by the app. The sung sections in particular are rough. Names and boundaries can be off. Listen and check.
- **Groove Check values** are guides. They do not judge how well you play.
- **Tab read from a photo or PDF** is a draft. Every bar is marked "?" until you check it against the original page.

Nothing in the app is shown as a certainty. Trust your ears over the numbers.

### 4-3. Rights are your responsibility

Whether you may capture or process a sound depends on the rights in the recording and on the terms of the service that plays it. The fact that a computer can capture a sound does not mean you may use it. Use only audio you are allowed to use.

Audio files with DRM (copy protection) cannot be opened, and protected sound may not be captured.

### 4-4. What is saved and what is not

- During normal playback the app does not save the song it captures, or the separated sound. Audio only passes through memory.
- When your computer cannot keep up, the app can store sound before playing it. That sound stays in memory only. It is thrown away when playback ends, when you switch separation off, or when you quit.
- What the app does save:
  - **Your own recordings.** Only what your microphone picks up, never the song. To line a take up with the song later, it saves a set of features that cannot be turned back into sound.
  - **Tabs, saved ranges and loops, and settings.**
  - **Performance measurements**, only when "Save performance measurements" is on. These are numbers, not audio.
  - **File history.** The names and locations of audio files you opened yourself.
  - **Separated sound for transcription (if you use the experimental feature).** The separated sound of the range you selected is kept on your computer and replaced when the next transcription is finished.
- Where it is kept: on the Mac, `~/Library/Application Support/OtoWake BG/`; on Windows, `%APPDATA%\OtoWake BG` and `%LOCALAPPDATA%\OtoWake BG`.
- You can delete saved information from inside the app (your recordings, the measurement history and the file history).

### 4-5. Experimental features

Features marked "Experimental" are still being tried out.

- **Groove Check.** Results depend on how well the song was separated. If separation goes badly, the numbers are not reliable either.
- **AI transcription (MCP).**
  - The transcription is not done inside the app. The AI assistant you set up does it. The app alone does not transcribe.
  - What the app prepares for the assistant is numbers: beats, note names and note candidates. The app does not send audio on its own. However, the separated sound of the range you selected is kept on your computer, and your assistant can ask for it, up to 30 seconds at a time. What your AI service does with that sound is governed by its own terms. Check them before you use this.
  - The note candidates are picked from the audio by a simple method and are not very accurate, so the AI's transcription can contain many wrong notes and fingerings that cannot be played. Always check it by ear.
  - On the Mac, the "Ask AI to Transcribe" buttons are not shown in the player at first. In Advanced Settings > "General" > "MCP settings (experimental)", switch on "Show “Ask AI to Transcribe” buttons in the player".

### 4-6. Computer speed and delay

Separating in real time takes a reasonably capable computer.

- Sound appears a few seconds, sometimes more than ten, after you switch separation on. For an audio file the app separates the song twice and averages the results, so it takes about 15 seconds (switching that off in Advanced Settings saves 6 to 7 seconds). Even after it starts, you hear the separated sound later than the original. With video, the sound lags behind the picture.
- When processing cannot keep up (when one chunk takes 80% or more of its 5-second slot), the app switches to buffered playback by itself. Buffered playback takes longer to start, and you cannot record yourself while it is in use.
- In Advanced Settings > "Separation", "Playback" lets you choose the method (Mac: "Auto", "Always real time", "Always buffer"; Windows: "Auto", "Real time", "Buffered playback"). If you force real time on a slow computer, the sound breaks up.
- A change to a volume, a part or the key is heard a moment later.
- This release has no list of tested computers.

### 4-7. Permissions the app asks for

- **Capturing Mac audio.** macOS asks permission to capture what the Mac plays. You grant it in System Settings > Privacy & Security > Screen & System Audio Recording. The captured sound is not saved.
- **Microphone.** Asked for when you record yourself. Only the microphone is saved. On Windows, allow desktop apps to use the microphone in Windows settings.
- **Camera.** Used only when you photograph tab. On the Mac it is a nearby iPhone camera (Continuity Camera); on Windows it is "Scan with camera" in the tab window. Only the photo is kept.
- **Controlling Music and other players (Mac).** Used to read the song title and position, and to move a player back for loops. Asked for when needed.

### 4-8. Using the numbers and transcriptions

- Check by ear before you put a measurement or a transcription into teaching material or hand it to others.

## 5. Credits and licences

### Material the separation model was trained on

The separation model is trained only on material that may be used for it. Credits for works that require attribution (CC BY and similar) are collected in the [credit list](../credits.md).

### Third-party software

The main third-party components used by the apps in this release are below. The full licence texts come with the app.

| Component | Licence | Used in |
|---|---|---|
| ONNX Runtime | MIT (the DirectML part is under Microsoft's own licence) | Windows |
| NAudio | MIT | Windows |
| SoundTouch.Net | LGPL-2.1 or later | Windows |

## 6. Feedback

Send comments and bug reports by direct message, to either of these:

- X: a direct message to @OtoWakeBG
- Substack: a direct message

We do not take feedback by email.

When you report a problem, it helps to include:

- Your OS and version, and your Mac model or your PC's CPU and GPU
- What you did and what happened
- On Windows, the text copied by "Copy Diagnostics" on the "Diagnostics" tab of Settings. It contains no audio or song names, but file locations can contain your user name, so read it before you send it. On the Mac, use "Copy Details" on the error message.
