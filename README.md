# Layers — v1.0.0

A Home Screen wallpaper overlay studio. Pick a wallpaper, toggle visual effects,
preview the result, save reusable layouts, and export the finished image.
Set the exported image as your wallpaper in **Settings > Wallpaper**.

iOS does not allow apps to draw on the Home Screen, so all effects are baked
into the exported wallpaper image at the exact positions where your Home
Screen icons sit.

## Install (easy way)

1. Download the unsigned `.ipa` from [Releases](https://github.com/mikevillarroel/layers/releases).
2. Sign it with [ESign](https://esign.yyyue.xyz), SideStore, or AltStore using your own certificate.
3. Install it on your iPhone.

## Build from source (test build)

1. Unzip this archive on your Mac.
2. Open `Layers.xcodeproj` in Xcode.
3. In the project editor, select the **Layers** target > **Signing & Capabilities**,
   and pick your Team.
4. Connect your iPhone, select it as the run destination, and press **⌘R**.
5. Look for **v0.1.0-test1** at the bottom of the Build screen to confirm
   you are running this build.

## How it works

- **Build screen**: choose a wallpaper from Photos, toggle effects
  (Icon borders, Icon glow, Depth shadow, Dark plates, Hide notch, Dock tint)
  and fine-tune each with sliders. Tap **Preview**.
- **Preview screen**: see the composited wallpaper, **Save layout** to reuse
  the effect settings later, or **Export** to save the finished wallpaper
  to Photos.
- The icon grid (4 × 6) is computed at runtime from your screen size, so it
  adapts to any iPhone from the 13 to the latest — including Display Zoom.

## Effects

All effects are generated procedurally in code (Core Graphics + Core Image).
No external image assets. Names are our own.

## Notes

- Test numbering: this is `v0.1.0-test1`. Only an explicit approval earns a
  release number.
- Nothing in this build is published anywhere — test builds go through chat.
