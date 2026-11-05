# Dragon Block 1000

Keep an existing DB1000 pack updated without downloading the entire pack again.

## Automatic updates from your normal Play button

Download [DB1000 Startup Updater](https://github.com/BloodMuffin618/db1000-updates/releases/latest/download/DB1000-Startup-Updater.zip) and extract it. Close Minecraft, then copy **`!DB1000-Updater.jar`** into your instance's `mods` folder beside **`DB1000-Release-1.0.jar`**. Keep the leading `!` and both filenames. Install this small addon once in each instance you use.

Now press **Play in Minecraft Launcher or Prism** as usual. During early Forge startup, the addon checks the stable release, downloads an update only when needed, verifies its SHA-256 and size, and replaces DB1000 before the main mod loads. Minecraft then continues in the same launch. No separate launcher app, launch command or GitHub sign-in is required.

The full DB1000 pack and Forge 1.7.10 must already be installed. This addon updates DB1000; it does not install the full pack or other dependencies. Older valid DB1000 builds without embedded release metadata are supported.

If Prism already has the old DB1000 updater in **Edit Instance → Settings → Custom Commands → Pre-launch command**, remove only that DB1000 command when switching to this addon. Preserve unrelated commands. Do not install the startup addon on a dedicated server.

A failed check or download stops startup with an explanation and preserves the installed mod. Fix the issue and press Play again. Interrupted replacements recover from one verified rollback stored outside `mods`. The addon does not replace a JAR already loaded by Minecraft. Future startup-addon changes may require replacing this small JAR; it automatically manages only the main DB1000 mod.

## Optional legacy launcher

Download [Dragon Block 1000 Setup.exe](https://github.com/BloodMuffin618/db1000-updates/releases/latest/download/Dragon.Block.1000.Setup.exe), run it, choose an install folder with **Browse**, and choose **Install**. It adds **Dragon Block 1000** to your desktop with the Shenron icon. You can send that single installer file to friends.

The full DB1000 pack must already be installed once. This installer adds the launcher; it does not install Minecraft, Forge or the full pack. Players do not need a GitHub account.

Open **Dragon Block 1000**, choose your client folder and launcher, and press **Play DB1000**:

- **Prism:** updates the mod, then starts the selected instance through Prism.
- **Regular Minecraft Launcher:** updates the mod, then opens Minecraft Launcher. Select the DB1000 profile for that game folder and press Play there.

Your existing launcher handles Minecraft sign-in. Close Minecraft before updating. Without the startup addon above, opening the original Minecraft shortcut bypasses this older external updater.

## Portable alternative and Prism's Play button

The [portable launcher ZIP](https://github.com/BloodMuffin618/db1000-updates/releases/latest/download/DB1000-Updater-Setup.zip) is also available. Extract the whole ZIP and open **Dragon Block 1000.exe**; the executable needs its bundled files.

The older Prism setup can also install a pre-launch command. Use the startup addon above for the simpler ordinary-Play workflow; do not configure both mechanisms together.

## What updates

The update channel manages **mods/DB1000-Release-1.0.jar only**. The startup addon is a separate one-time installation. Other mods, resource packs, shaders, settings, keybinds, worlds, screenshots, server lists and Xaero maps are unchanged. Downloads are staged and checked by size and SHA-256 before replacing the installed mod. An unchanged mod is not downloaded again.

The mod keeps the Release 1.0 filename; a build ID and checksum identify each update. Launcher updates are available through a new installer download. This launcher does not silently replace its own executable.

The private server update channel is separate and requires the owner's GitHub access. Do not use the client updater on a dedicated server.

## Update engine

The startup addon uses a standalone Java 8 updater during Forge coremod discovery. The optional older launcher uses [packwiz-installer](https://github.com/packwiz/packwiz-installer) v0.5.14 and [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap) v0.0.3, pinned for Java 8. Notices are included. Account credentials are never included in downloads.
