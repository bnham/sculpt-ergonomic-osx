I recently bought a Microsoft Sculpt Ergonomic Desktop keyboard and mouse set
for use with my Mac OS X laptop. Unfortunately, Microsoft has dropped support
for their keyboard and mice via their Intellipoint driver as of Lion, so to use
some of the extra keys on the mouse, you have to resort to third-party utilities
like [Karabiner](https://pqrs.org/osx/karabiner/) or
[BetterTouchTool](https://www.boastr.net).

This repo contains a private.xml file for use with Karabiner that remaps the
following keys:

- Context menu key (the key to the right of the right Alt button) to the option
  key.
- Windows button on the mouse to either mouse5 (in case you want to use another
  tool like BetterTouchTool to customize further) or Mission Control. Note that
  BetterTouchTool is unable to recognize the Windows button on this mouse by
  itself, which is why is why the mouse5 remapping is useful.
- Back button on the mouse to `Cmd + [`, which is the default shortcut for back
  in many apps.
- Left scroll and right scroll to `Cmd + Shift + [` and `Cmd + Shift + ]`
  respectively. This maps to previous/next tab in many apps.

After loading the private.xml file in Karabiner, you can use Karabiner's GUI to
select which of these key remappings to use.

---

Karabiner stopped working because of the keyboard driver architecture changes at macOS Sierra. Thus, [Karabiner-Elements](https://github.com/tekezo/Karabiner-Elements#karabiner-elements) was made from scratch for new macOS.

This repo contains a karabiner.json file for use with [Karabiner-Elements](https://pqrs.org/osx/karabiner/json.html) that remaps the following keys:

- left_gui (equal to \`left_command\`) -> left_contrl
- left_control -> legt_gui (equal to \`left_command\`)
- `f1`...`f12` key codes to macOS counterpart

You can now use the standard/non-macOS "copy and paste" workflow and `f*` keys.

Upload the file to ~/.config/karabiner/karabiner.json then you can use Karabiner's GUI to
select which of these key remappings to use.

[karabiner.json Reference Manual](https://pqrs.org/osx/karabiner/json.html)


