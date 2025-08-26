<h1 align=center>INSTALLATION INSTRUCTIONS</h1>

---

## EXPLORER SETUP

### Quick Access:
1. Open the Windows Registry using `win + r` - `regedit`
2. Navigate to the section:
```bash
HKEY_CLASSES_ROOT\CLSID\{679f85cb-0220-4080-b29b-5540cc05aab6}\ShellFolder
```
4. Right-click on the name of this section, select "Permissions" from the menu.
5. Then click **Advanced**.
6. In the **Owner** field - click **Edit**, in the next window enter **Administrators** and click `Ok`, then in the next window `Ok`.
7. Ensure that **Administrators** is selected in the list, set **Full Control** for this group, and click `Ok`.
8. Set the `Attributes` parameter to ```a0600000``` (in hexadecimal).
9. Pin the required folders and shortcuts to the Quick Access panel.

### Gallery
1. Navigate to the section:
```bash
HKEY_CURRENT_USER\Software\Classes\CLSID
```
3. Create a subkey named:
```bash
{e88865ea-0e1c-4e20-9aa6-edcd0212c87c}
```
7. Create a DWORD parameter named `System.IsPinnedToNameSpaceTree`. Value - **0**.

### OneDrive
1. Navigate to the section:
```bash
HKEY_CLASSES_ROOT\CLSID\{018D5C66-4533-4307-9B53-224DE2ED1FE6}
```
3. Change the `System.IsPinnedToNameSpaceTree` parameter to **0**.

---

# Theme Installation

Follow the installation instructions from niivu<br>
[**Tokyo Night Theme**](https://www.deviantart.com/niivu/art/Tokyo-Night-for-Windows-11-970381220)<br>
[**Instructions**](https://www.deviantart.com/niivu/art/Installing-Windows-Themes-UPDATED-708835586)<br>

---

# Windhawk
1. Install [**Windhawk**](https://windhawk.net/)
2. Install the extensions **Taskbar height and icon size**, **Windows 11 Notification Center Styler**, **Windows 11 Start Menu Styler**, and **Windows 11 Taskbar Styler**.
3. Use the configs from [the folder](.config/windhawk) and apply them in the extensions.

---

# PowerToys
Use the screenshots from [the folder](.config/powertoys) to configure PowerToys.

---

# Visual Studio Code
1. Use the shortcut `ctrl + shift + p` and type:
```bash
> Preferences: Open User Settings (JSON)
```
3. Use the config - [VSCode config](.config/vscode/settings.json).
4. Use the shortcut `ctrl + shift + p` and type:
```bash
> Reload Vibrancy
```
6. Restart VS Code.

---

# Firefox
1. Install the theme [**Tokyo Night**](https://addons.mozilla.org/ru/firefox/addon/tokyo-night-theme-for-firefox/) and activate it.
2. Install the extension [**NightTab**](https://addons.mozilla.org/ru/firefox/addon/nighttab/).
3. Go to settings and select NightTab for new tabs.
4. Open a new tab, go to settings, under `Data` - `Restore` and use the file - [NightTab config](.config/firefox/nighttab.json).

---

# Windows Terminal
1. Go to settings.
2. Click on the `Open JSON file` button with the gear icon.
3. Replace the content with - [Terminal config](.config/terminal/settings.json).

---

# Starship
1. Use the command `winget install Starship` in PowerShell.
2. Download the file to `~/.config/` - [Starship config](.config/starship.toml).
3. Enter the command:
```pwsh
$ENV:STARSHIP_CONFIG = "$HOME\.config\starship.toml"
```
4. Use the command:
```pwsh
start $PROFILE
```
5. Add the following line to this file:
```pwsh
Invoke-Expression (&starship init powershell)
```

# Wallpaper
I use a picture from [Need for Speed™ Heat Deluxe Edition Upgrade](https://www.ea.com/games/need-for-speed/need-for-speed-heat/buy/addon/need-for-speed-heat-deluxe-edition-upgrade) - [Image](https://drop-assets.ea.com/images/20Dwl4UUku94FKgNAOHw91/ad3e2b12b09b78f62fca028072d3f687/OTMM_57492153_NFS_Heat_Deluxe_Key_Art_HORIZONTAL_RGB_10_.jpg?im=AspectCrop=(16,9),xPosition=0.583125,yPosition=0.5611111111111111;Resize=(1280)&q=85)
