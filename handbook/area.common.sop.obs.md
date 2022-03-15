---
id: 734ppnlkvwse5wb2crjryqj
title: OBS
desc: >-
  Using Open Broadcaster Software (OBS) for recording sessions with the purpose
  of either uploading to YouTube or sending directly to users, such as
  optionally recorded onboarding sessions.
updated: 1646681456916
created: 1646678329714
---

## Summary

Using [Open Broadcaster Software (OBS)](https://obsproject.com/) for recording sessions with the purpose of either uploading to YouTube or sending directly to users, such as optionally recorded onboarding sessions.

This SOP covers a minimal setup for sharing a screen, and for setting up audio. Reference links are also included for more in-depth configurations.

## Prereqs

Install [OBS Studio](https://obsproject.com/), free software that can work on MacOS, Windows, and Linux.

## Steps

### Profile

- Profile -> New
- Name it what you'd like, such as `Dendron Recording`
- Auto-configuration wizard can be done, with a focus on recording rather than streaming

### Sources

This configuration assumes a single scene for a minimal setup. Two sources need to be added:
- **Audio Input Capture**
- **Screen Capture**
- Optional: **Video Capture Device** (webcam, etc.)

> For more details on the filters used for Audio and Video, reference the [OBS tutorial: Audio and video filters in OBS Studio (Guide)](https://projectobs.com/en/tutorials/audio-video-filters-obs-studio-guide/).

#### Audio Input Capture

- Right-click inside the `Sources` window -> `Add` -> `Audio Input Capture`
- Create new
- Select microphone of choice
- Once added, you may want to _rename_ to a more readable representation of the selected mic.
  - Right-click -> `Rename`

Now, it's time to configure _filters_. These are important in keeping out unnecessary noise, and providing a higher quality audio experience.

> **NOTE:** These settings were pulled from a variety of articles, and seemed to work well for several streamers and general users of OBS.

- Right-click the new `Audio Input Capture` source you just added
- Select `Filters`
- Add: `Noise Suppression`
  - `RNNoise` is preferred, but either work depending on the specs of your device
- Add: `Noise Gate`
  - **Close Threshold:** -60.00 d
  - **Open Threshold:** -50.00 d
  - **Attack Time:** 25ms
  - **Hold Time:** 50ms
  - **Release Time:** 50ms
- Add: `Compressor (Limiter)`
  - **Ratio:** 10.00
  - **Threshold:** -6.00 dB
  - **Attack:** 1ms
  - **Release:** 15ms
  - **Ouput Gain:** 0.00 dB
  - **Sidechain/Ducking Source:** None
- Add: `Compressor`
  - **Ratio:** 3.00
  - **Threshold:** -24.00 dB
  - **Attack:** 3ms
  - **Release:** 15ms
  - **Output Gain:** 6.00 dB
  - **Sidechain/Ducking Source:** None

There should also be an `Audio Mixer` panel, which should show:
- `Desktop Audio`
- `(Your Microphone)`

You will want to likely have the `Desktop Audio` be lower than your own microphone, since you won't necessarily know how loud another microphone may be.

An example setup used:
- **Desktop Audio:** -5.3 dB
- **Yeti Microphone:** -0.0 dB

#### Screen Capture

- Right-click inside the `Sources` window -> `Add` -> `Screen Capture`
- Create new

Your screen should show the contents of the default monitor screen. If you are intending to share a different screen, this can be modified via the `Properties` of the `Screen Capture` source.

### OBS General Settings

> **NOTE:** This may differ depending on your hardware. Tweaks should be made if certain audio or video issues happen in your recordings. It's generally advised that you run test sessions to get familiar with OBS, and if the audio or video results of your recordings seem off in any way, that modifications to your settings are evaluated.

- File -> Settings
- Output
  - Streaming (Optional)
    - **Output Mode:** Simple
    - **Video Bitrate:** 2500 Kbps
    - **Encoder:** Hardware (NVENC)
    - **Audio Bitrate:** 160
  - Recording
    - **Recording Path:** Enter preferred output path
    - **Recording Quality:** High quality, medium file size
    - **Recording Format:** mkv
    - **Encorder:** Hardware (NVENC)
- Audio
  - General
    - **Sample Rate:** 48kHz
    - **Channels:** Mono
  - Global Audio Devices
    - **Desktop Audio:** Default
    - _All other options:_ Disabled
  - Meters
    - **Decay Rate:** Fast
    - **Peak Meter Type:** Sample Peak
  - Advanced
    - **Monitoring Device:** Default
  - Hotkeys
    - Keep as defaults, unless wanting to customize
- Video
  - _These settings may depend on your display resolutions._
  - **Base (Canvas) Resolution:** 1920x1080
  - **Output (Scaled) Resolution:** 1920x1080
  - **Downscale Filter:** Bicubic (Sharpened scaling, 16 samples)
  - **Common FPS Values:** 60

### Recording and Converting Recordings

- There is a `Start Recording` in the `Controls` panel that will be capturing your active sources into an `mkv` file
- When the file is saved, `mkv` can be converted (or "remuxed") into other formats.
- Remuxing
  - File -> Remux Recordings
  - Select the recording under `OBS Recording` (can select multiple recordings)
  - Select `mp4` (standard format for uploading to YouTube, sharing, etc.)
  - Click `Remux`
  - The conversion should be fast, and will be default create the output in the same directory as the source video

## Another Example Configuration

An excellent video on using OBS Studio for streaming, scenes, sources, transitions, etc.
- [OBS For Brand New Streamers](Creating Scenes, Adding Custom Widgets, and MORE)](https://www.youtube.com/watch?v=EuSUPpoi0Vs)

The following is covered:

- Overview
- Setting Up Your First Scene
- Adding Cool Widgets
- Adding a Second Scene
- Transitions
- The Audio Mixer
- The Settings
- Switching Scenes w/ a Hotkey

Much of this applies to configuration setup for users that aren't streaming, just as much as it may be for those who are. This was the first video referenced when initially setting up OBS, before later creating this SOP.

### Quick reference

- The initial configuration wizard can be used for optimizing for streaming
- Twitch can be selected, and the API streaming key should be entered
  - **OPTIONAL**: Can stream against personal channel for testing, if setting up to stream to Twitch. OBS Studio provides a button that will go directly to the personal channel key location.
- At a minimum, there needs to be one **Scene** with the following sources:
  - **Video Capture Device**: For selecting your webcam, if wanting to include your face on the stream
  - **Mic/Aux** (or **Audio Input Capture** using your mic): For viewers to hear your voice
  - **Screen Capture**: To share targeted windows, desktops, etc.

## Related

- [How to setup OBS Studio for streaming](https://projectobs.com/en/tutorials/how-to-setup-obs-studio-for-streaming/)
