# Colorful (Simplified) — Anbernic RG353V Edition

A vibrant, system-coloured EmulationStation theme adapted for the **Anbernic RG353V** running **dArkOS**, optimised for its **640×480 (4:3)** display.

> **Fork Notice**
> This is a fork of [Colorful (Simplified) for ES-DE](https://github.com/anthonycaccese/colorful-simplified-es-de) by [anthonycaccese](https://github.com/anthonycaccese), which itself is a port of the original Colorful theme for Launchbox created by [viking](https://forums.launchbox-app.com/profile/70421-viking/) & [faeran](https://forums.launchbox-app.com/profile/76940-faeran/).
> If you are **not** using an RG353V or a device with a 640×480 screen and dArkOS, please use the [original theme](https://github.com/anthonycaccese/colorful-simplified-es-de) instead.

---

## Preview

> Screenshots below are from the upstream theme at 16:9. RG353V screenshots will be added here once captured on device.

| System View | Gamelist View |
| :---------: | :-----------: |
| ![System View](https://github.com/user-attachments/assets/9d1d32e0-77e2-4088-83ac-d73d64d675cc) | ![Gamelist View](https://github.com/user-attachments/assets/09cda077-22e4-4dc8-af38-dc289f82698f) |

---

## Installation

1. Copy this folder into your dArkOS themes directory:
   ```
   /roms/themes/
   ```
2. The folder should be named `es-theme-colorful` (or whatever you prefer).
3. In EmulationStation, go to **Main Menu → UI Settings → Theme Set** and select this theme.
4. Restart EmulationStation if the theme does not appear immediately.

---

## What Changed in This Fork

This fork adapts the upstream theme specifically for the RG353V's 640×480 screen and dArkOS's EmulationStation. Key changes include:

### Layout & Resolution Fixes
- **Battery indicator** repositioned and font-sized to match the clock, preventing overflow on the 640px-wide screen
- **Battery icon paths** corrected (were pointing to a wrong directory)
- **System description** repositioned so it no longer bleeds into the bottom help bar
- **Gamelist line spacing** reduced (`1.683 → 1.4`) to display more game titles on the small screen
- **Help bar** font size tuned to prevent overflow with 4–5 items on 640px

### Bug Fixes (from upstream)
- `fontSemiBold` variable was self-referencing — fixed to point to `Gilroy-SemiBold.ttf`, restoring the correct gamelist font
- `gameMetadataBackground` pointed to a non-existent `_inc/` directory — fixed to `./_art/assets/`
- Star rating unfilled icon had a typo (`iocn-star-unfilled`) — corrected to `icon-star-unfilled`
- Broken non-functional font-size subset removed (referenced subdirectories that didn't exist)

### dArkOS Compatibility
- Added `iconOptions` menu icon for the dArkOS-specific Options menu entry

---

## Color Schemes

The theme uses a per-system accent colour automatically. There is no manual color scheme switcher in this fork.

Each system folder (`nes/`, `snes/`, `gba/`, etc.) defines its own `systemBackgroundColor` to match the Colorful art set.

---

## Credits

- Original Colorful artwork by [viking](https://forums.launchbox-app.com/profile/70421-viking/) & [faeran](https://forums.launchbox-app.com/files/file/2081-colorful-bigbox-theme)
- ES-DE port by [anthonycaccese](https://github.com/anthonycaccese)
- Additional system artwork sourced from [g-spawn](https://github.com/g-spawnPL)'s [ckau-book](https://github.com/CkauNui/ckau-book) theme (edited for transparency)
- OpenBOR sprites by [DOA687](https://www.deviantart.com/doa687)
- M.U.G.E.N. sprites by [mpadillathespriter](https://www.deviantart.com/mpadillathespriter)
- EasyRPG artwork by [SeraphCircle](https://twitter.com/SeraphCircle)
- Doom artwork by [azakachi-rd-17](https://www.deviantart.com/azakachi-rd-17)
- Folder icons sourced from [FontAwesome](https://fontawesome.com/search?o=r&m=free)

---

## License

[Creative Commons CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
You are free to share and adapt this theme for non-commercial purposes, as long as you give appropriate credit and distribute your changes under the same license.
