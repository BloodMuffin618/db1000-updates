# Dragon Block 1000 updates

Updates for an existing DB1000 installation. You do not need to download the full pack again.

## Players on Windows

Download **DB1000-Updater-Setup.zip** from [the latest release](https://github.com/BloodMuffin618/db1000-updates/releases/latest), extract the complete folder, and open **Dragon Block 1000.exe**.

Choose your regular client or Prism installation. The launcher verifies and updates the DB1000 mod before launching. Prism starts the selected game directly. Regular mode opens Minecraft Launcher; use its DB1000 profile and press Play.

For automatic updates when using Prism's own Play button, run **Setup-DB1000.cmd** once and choose Prism. For the regular launcher, use Dragon Block 1000 or the desktop shortcut created by setup. Launching the original Minecraft shortcut directly does not run this updater.

This update channel currently manages **mods/DB1000-Release-1.0.jar only**. Other mods, resource packs, shader packs, settings, keybinds, worlds, screenshots, servers, and Xaero maps are not changed. You must already have the DB1000 pack installed. Close Minecraft before updating.

The setup download contains no account credentials. Players do not need a GitHub account. Minecraft sign-in is handled by the launcher you already use.

## Releases

The mod keeps its Release 1.0 filename. Updates are identified by a build ID and SHA-256 checksum. A changed mod downloads as a complete JAR; unchanged files are not downloaded. Downloads are staged and checked before the installed file is replaced.

The private server update channel is separate and requires owner access. Do not use the client updater on a dedicated server.

## Update engine

The updater uses [packwiz-installer](https://github.com/packwiz/packwiz-installer) v0.5.14 and [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap) v0.0.3, pinned for Java 8. Third-party notices are included in the setup ZIP.
