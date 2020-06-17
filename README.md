
## Sheffield-Grub2-Theme
Sheffield Grub2 Theme with Papirus Icon Pack
![sheffield grub theme without loading bar](https://raw.githubusercontent.com/osmanonurkoc/Sheffield-Grub-Theme/master/sheffield_grub.png)
## Installation:

**Installer:**

Just run this command in your terminal.

    $ sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/osmanonurkoc/Sheffield-Grub-Theme/master/install.sh)"

**Manual:**

 - Clone the repository `git clone https://github.com/osmanonurkoc/Sheffield-Grub-Theme.git`
 - Copy the folder **Sheffield/** in the themes folder where GRUB is installed: (/boot/grub/themes)
 - Edit  **/etc/default/grub**  and place the SHEFFIELD theme path with your text file  **theme.txt**
`GRUB_THEME="/boot/grub/themes/Sheffield/theme.txt"`
 -  Generate your grub configuration file again (sudo update-grub or grub-mkconfig)
 - That's all

## How to config theme:

Run command `sudo xed /boot/grub/grub.cfg`

*For add missing icons to grub menu entries:*

 1. Find first`menuentry "` line
 2. Add `--class "iconname"` to end of the `menuentry "entry-name"` 
 3. Look [icons](https://github.com/osmanonurkoc/Sheffield-Grub-Theme/tree/master/Sheffield/icons) for "iconname"
 4. Save file and reboot

It should look like the following at the end of the processes.
  `menuentry "Linux Mint 20 Cinnamon" --class linuxmint`

*For set  grub menu default entry:*

 1. Find `set default="`
 2. Add value in `set default="right-here"` to you want be a default entry
 3. For example: `set default="Linux Mint 20 Cinnamon"` like be for linux mint

 
