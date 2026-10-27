# Movable HUD

Move the HUD by holding its footer.

Hold the HUD's footer (the level, class and weight line) and drag to move the HUD anywhere on screen. Switch: Options > UI > Add-ons.

An add-on for [ROSE Mod Launcher](https://github.com/Zurnny/Rose_Mod_Launcher), for the game's default UI and the Steampunk UI theme. Without the launcher, copy the `Data` folder from `files` into your ROSE Online folder.

## Install
1. Download this repo (Code > Download ZIP) and open it.
2. Copy the **Movable HUD** folder into `Launcher Mods` in your ROSE Online folder.
3. Open the launcher, press **Mods**, tick **Movable HUD**, and restart the game.

It updates itself from this repo whenever the launcher opens.

## Works with the other add-ons
Every add-on works on its own, and any mix of them works together. Add-ons
that change the same window (Options, the HUD, the party and group windows)
carry the very same copy of that file, and each part only runs while its own
add-on is installed: each add-on puts a small marker file in
`Data/ui/sp_addons/`, which the launcher removes again with the add-on.
In **Options > UI > Add-ons** each installed add-on adds its own line, one
under the other, in the order they are listed there.

## Default UI or Steampunk
Each window it changes holds both looks: the game's own and the [Steampunk UI](https://github.com/Zurnny/SteamPunk) theme's. When the window opens it checks whether Steampunk is installed (`styles/steampunk.css`) and uses that look, so it works with either one, with or without the launcher. With Steampunk, the Steampunk theme's own features stay on too.

The switches are saved in `sp_addons.txt` in the ROSE Online folder. The Ice UI
theme uses the same file; both keep each other's settings.

## Files it changes
- `Data/ui/themes/rose/game/hud.html`
- `Data/ui/themes/rose/game/options_bgfx.html`
- `Data/ui/themes/rose/styles/sp_addons_steampunk_sprites.css` (Steampunk look, shared by the add-ons)
- `Data/ui/sp_addons/hud_move.txt` (marker)

Turning it off in the launcher puts the game's own files back.
