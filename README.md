# Dragon Block 1000

Keep an existing DB1000 pack updated without downloading the entire pack again.

## Install the launcher

Download [Dragon Block 1000 Setup.exe](https://github.com/BloodMuffin618/db1000-updates/releases/latest/download/Dragon.Block.1000.Setup.exe), run it, choose an install folder with **Browse**, and choose **Install**. It adds **Dragon Block 1000** to your desktop with the Shenron icon. You can send that single installer file to friends.

The full DB1000 pack must already be installed once. This installer adds the launcher; it does not install Minecraft, Forge or the full pack. Players do not need a GitHub account.

Open **Dragon Block 1000**, choose your client folder and launcher, and press **Play DB1000**:

- **Prism:** updates the mod, then starts the selected instance through Prism.
- **Regular Minecraft Launcher:** updates the mod, then opens Minecraft Launcher. Select the DB1000 profile for that game folder and press Play there.

Your existing launcher handles Minecraft sign-in. Close Minecraft before updating. Opening the original Minecraft shortcut directly bypasses this updater.

## Portable alternative and Prism's Play button

The [portable launcher ZIP](https://github.com/BloodMuffin618/db1000-updates/releases/latest/download/DB1000-Updater-Setup.zip) is also available. Extract the whole ZIP and open **Dragon Block 1000.exe**; the executable needs its bundled files.

To update automatically from Prism's own Play button, run **Setup-DB1000.cmd** once and choose Prism. The refreshed DB1000 Prism pack already includes this hook.

## What updates

The update channel manages **mods/DB1000-Release-1.0.jar only**. Other mods, resource packs, shaders, settings, keybinds, worlds, screenshots, server lists and Xaero maps are unchanged. Downloads are staged and checked by size and SHA-256 before replacing the installed mod. An unchanged mod is not downloaded again.

The mod keeps the Release 1.0 filename; a build ID and checksum identify each update. Launcher updates are available through a new installer download. This launcher does not silently replace its own executable.

The private server update channel is separate and requires the owner's GitHub access. Do not use the client updater on a dedicated server.

## Update engine

Uses [packwiz-installer](https://github.com/packwiz/packwiz-installer) v0.5.14 and [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap) v0.0.3, pinned for Java 8. Notices are included. Account credentials are never included in downloads.
