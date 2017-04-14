# About

Helio is a minimal theme for the GRUB bootloader.

![Preview](preview/Preview.png)

# Installation
To install the theme, place the "helio" folder in the GRUB themes folder, usually located at `/boot/grub/themes`, E.g.:

    git clone https://github.com/Tomha/GrubThemeHelio
    sudo cp -r GrubThemeHelio/helio /boot/grub/themes/

**Activating the Theme:**
To use the theme, set the `GRUB_THEME` line in the GRUB config file, usually located at `/etc/default/grub`, e.g.: `GRUB_THEME=/boot/grub/theme/helio/theme.txt`.

**Low Resolution Fix:**
If GRUB defaults to a very low resolution you can try forcing a higher resolution for a better apperance, and to fit more entries on the screen without having to scroll.
1. Reboot into grub and press `c` to get the GRUB command prompt
2. Run `vbeinfo` to list available resolutions
3. Set the `GRUB_GFXMODE` line in the GRUB config file as per above, e.g.: `GRUB_GFXMODE=1600x1200`
