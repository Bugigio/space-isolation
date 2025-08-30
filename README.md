# Space Isolation
A GRUB theme based on the main menu of the 2014 survival horror game Alien: Isolation™.

![Preview](preview.jpg "Space Isolation GRUB2 Theme Preview")

## Installation
> [!IMPORTANT]
> This theme is a WIP **only supporting 2560x1440 and 1920x1080** resolutions. It will not look optimal on different resolutions. Feel free to add support for your resolutions using [this contribution guide](CONTRIBUTING.md).

### Arch Linux
1. Rename the directory with your resolution to `space-isolation`
2. Copy this directory to `/boot/grub/themes`
    ```zsh
    cp -r /path/to/space-isolation /boot/grub/themes
    ```

2. In `/etc/default/grub`, set `GRUB_THEME=` to `/boot/grub/themes/space-isolation/theme.txt` and make sure `GRUB_TERMINAL_OUTPUT="gfxterm"`
3. Update GRUB
    ```zsh
    grub-mkconfig -o /boot/grub/grub.cfg 
    ```

### Ubuntu/Debian
1. Rename the directory with your resolution to `space-isolation`
2. Create the following directory if it doesn't exist already
    ```zsh
    mkdir /boot/grub/themes
    ```
3. Copy the directory you renamed `space-isolation` to `/boot/grub/themes`
    ```zsh
    cp -r /path/to/space-isolation /boot/grub/themes
    ```
4. Open `/etc/default/grub` as `root`, set `GRUB_THEME=` to `/boot/grub/themes/space-isolation/theme.txt` and make sure `GRUB_TERMINAL_OUTPUT="gfxterm"`. Add those variables if you didn't find them. Last set `GRUB_GFXMODE=` to the resolution you've chosen (`1920x1080` or `2560x1440`) and uncomment it.
5. Update GRUB
   ```zsh
   update-grub
   ```
   

## Contribution
Feel free to contribute to this project using [this contribution guide](CONTRIBUTING.md). Leave a review on [Pling](https://www.pling.com/p/2296342/).
