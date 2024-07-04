# Sharks

[TOC]

------

## Droid

**1. (On Phone and PC) On a compatible Phone, install Lineage OS (Custom ROM)**

​       1.0.1. Install adb on your Computer `yay -S adb` then restart `sudo reboot`

​       1.0.2. Update oder Downgrade Phone to **Android 13**

​       1.0.3. On  your Phone go to `/Settings/About the Phone/Build-Number` and press it a couple of Times, till "**Developersettings already activated**" appears

​       1.0.4. Go to /`Settings/System/Developeroptions`, activate it then after all options unfold, activate *USB-Debugging*

​       1.0.5. Now plug your Phone to Computer, then change the USB Options from `Charging` to `File Transfer`

​       1.0.6. Your Phone should appear in your File-Browser now, go to the phone's directory, open the Terminal within this directory and type `adb -d reboot bootloader`

​       1.0.7.  Your Phone shuts down. Wait a bit and u should find your phone in **"Fastboot Mode"** . In the Terminal type `sudo fastboot devices` and it should print out the name of your Phone

​       1.0.8. If not begin start over, if there's one type `sudo fastboot flashin unlock`

​       1.0.9. Now the Device is doing something, jus accept anything and wait till it starts up again

​       1.1.0. Download the  `vendor_boot.img`  Version for your phone, from the Lineage Webpage onto your PC (directory doesnt matter)

​       1.1.1 Connect your phone again and type `adb -d reboot`

​       1.1.2 When in Fastboot Mode, type `sudo fastboot flash vendor_boot ~/directory/of/vendor_boot.img`. 

​       1.1.3. Done

**2. Block Ad's and Distractions** 

​     2.1 Type `adb root`

​     2.2 Then type `adb remount`

​     2.3 Download this [File](https://github.com/marlonivo/.config/blob/5d397e113ac4f6d172775a88c03c39ea72ce6987/block-disctractions.txt) in a directory

​     2.4 Type: `adb push /etc/hosts /system/etc/hosts`

**3. Download F-Droid and Apps** 

`Orgzly Revived; aio-launcher; Nextcloud; AnkiDroid; DAVx³; Material-Files; KOReader; Syncthing-GTK; K-9 Mail; Mull; Collabora-Office; Notes; mAbook MuPDF-mini; Orbot; Seal; DNS66; Organic Maps`

------

## Desktop 

**1. Download [Artix ISO](https://artixlinux.org/download.php)** (if not familiar with setting up a graphical envirement yourself, installing a prefconfigured Graphic Server ISO like wayland is recommended)
     1.1 Flash the ISO on your USB Stick
     1.2 Plug the USB Stick into your Computer and follow trough the installation Process

**2. Download Yay, the Version Control System helper** (that thing keep's all of your Software up to date)
      2.1 Update anything:  `sudo pacman -Syyu`
      2.2 Install Git: `sudo pacman -S git`
      2.3 Install Yay:  `pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si`
      2.4 Reboot your system

**3. Download Utilities with Yay**

| Utilities                                                    | File Navigation                                              | Content Creation                                             | Studying                                                     | OS Tools                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| `virtualbox` - Virtual Machineware<br/>`timeshift` - Snapshot Tool<br/>`thunderbird` - Mail Client<br/>`flameshot` - Screenshot Tool<br/>`monero-gui` - Monero Wallet<br/>`electrum` - Bitcoin Wallet<br/>`electrum-ltc` - Litecoin Wallet<br/>`wget` - Download files from the web<br/>`gpartes` - Change Partition Size<br/>`htop` - Processor Tool<br/>`librewolf-bin` - Modern and safe Webbrowser | `syncthing` - Local File Syncing<br/>`nextcloud-client` - Cloud File Syncing<br/>`dolphin` - File Browser<br/>`mpv` - Video File Player<br/>`sxiv` - Photo File Viewer<br/>`zathura-pdf-mupdf` - PDF Viewer<br/>`libreoffice-still` - All Files <br/>`typora` - Markdown Files<br/> | `kdenlive` - Video Editing (opt. `python-vosk` - Sprachmodell)<br/>`gimp` - Photo Editing<br/>`audacity`  - Audio Editing<br/>`obs-studio` - Audio & Video Recorder | `anki` - SRS Software<br/>`goldendict` - Dictionary <br/>`calibre` - Ebook File Viewer & Manipulator<br/>`fcitx` - Inputlayout for languages | `dwm` - Window Tiling Manager<br/>`dwmblocks` - Configurable Bar<br/>`dmenu` - Menu for Software<br />`dunst` - Notificatio Deamon<br/>`unclutter` - Mouse Hide<br/>`pipewire` - Media Server <br/>`breeze` - Themes for Kde Software<br />`zsh` - Terminal<br/>`st` - Terminal |

**4. Sync & Configure Utilities**
  4.1 If you want to Configure them yourself feel free if not, you'll find all configs in a Folder called "Ricebowl" on this [page]()

**5. Block Ad's and Distractions**
   5.1 In terminal type: `sudo vim /etc/hosts` & [paste this](https://github.com/marlonivo/Config/raw/main/Block-Disctractions.txt) in.

