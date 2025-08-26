<h1 align=center>ИНСТРУКЦИИ ПО УСТАНОВКЕ</h1>

---

## НАСТРОЙКА ПРОВОДНИКА

### Быстрый доступ:
1. Откройте реестр Windows с помощью `win + r` - `regedit`
2. Перейдите в раздел:
```bash
HKEY_CLASSES_ROOT\CLSID\{679f85cb-0220-4080-b29b-5540cc05aab6}\ShellFolder
```
4. Нажмите правой кнопкой мыши по имени этого раздела, выберите пункт «Разрешения» в меню.
5. Далее нажмите **Дополнительно**.
6. В поле **Владелец** - **Изменить**, в следующем окне введите **Администраторы** и нажмите `Ок`, в следующем окне `Ок`.
7. Убедитесь, что в списке выбран пункт **Администраторы**, установите **Полный доступ** для этой группы и нажмите `Ок`.
8. Задайте параметру `Attributes` значение ```a0600000``` (в шестнадцатеричной системе счисления).
9. Закрепите на панели быстрого доступа требуемые папки и ярлыки

### Галерея
1. Перейдите в раздел:
```bash
HKEY_CURRENT_USER\Software\Classes\CLSID
```
3. Создайте подраздел с именем:
```bash
{e88865ea-0e1c-4e20-9aa6-edcd0212c87c}
```
7. Создайте DWORD параметр с именем `System.IsPinnedToNameSpaceTree`. Значение - **0**.

### OneDrive
1. Перейдите в раздел:
```bash
HKEY_CLASSES_ROOT\CLSID\{018D5C66-4533-4307-9B53-224DE2ED1FE6}
```
3. Измените параметр `System.IsPinnedToNameSpaceTree` на **0**

---

# Установка темы

Следуйте инструкциям по установке от niivu<br>
[**Тема Tokyo Night**](https://www.deviantart.com/niivu/art/Tokyo-Night-for-Windows-11-970381220)<br>
[**Инструкция**](https://www.deviantart.com/niivu/art/Installing-Windows-Themes-UPDATED-708835586)<br>

---

# Windhawk
1. Установите [**Windhawk**](https://windhawk.net/)
2. Установите дополнения **Taskbar height and icon size**, **Windows 11 Notification Center Styler**, **Windows 11 Start Menu Styler** и **Windows 11 Taskbar Styler**
3. Используйте конфиги из [папки](.config/windhawk) и используйте в дополнениях

---

# PowerToys
Используйте скриншоты из [папки](.config/powertoys) для настройки powertoys

---

# Visual Studio Code
1. Используйте сочетание клавиш `ctrl + shift + p` и введите:
```bash
> Preferences: Open User Settings (JSON)
```
3. Используйте конфиг - [VSCode конфиг](.config/vscode/settings.json)
4. Используйте сочетание клавиш `ctrl + shift + p` и введите:
```bash
> Reload Vibrancy
```
6. Перезайдите в VS Code

---

# Firefox
1. Установите тему [**Tokyo Night**](https://addons.mozilla.org/ru/firefox/addon/tokyo-night-theme-for-firefox/) и активируйте
2. Установите дополнения [**NightTab**](https://addons.mozilla.org/ru/firefox/addon/nighttab/)
3. Перейдите в настройки и выберите NightTab для новых вкладок
4. Откройте новую вкладку, перейдите в параметры, пункт `Data` - `Restore` и используйте файл - [NightTab конфиг](.config/firefox/nighttab.json)

---

# Windows Terminal
1. Перейдите в параметры
2. Нажмите на кнопку `Открытие файла JSON` со знаком шестерни
3. Замените содержимое на - [Terminal конфиг](.config/terminal/settings.json)

---

# Starship
1. Используйте команду `winget install Starship` в powershell
2. В папку `~/.config/` загрузите файл - [Starship конфиг](.config/starship.toml)
3. Введите команду:
```pwsh
$ENV:STARSHIP_CONFIG = "$HOME\.config\starship.toml"
```
4. Используйте команду:
```pwsh
start $PROFILE
```
5. Добавьте в этот файл строку:
```pwsh
Invoke-Expression (&starship init powershell)
```

---

# Обои
Я использую картинку из [Need for Speed™ Heat Deluxe Edition Upgrade](https://www.ea.com/games/need-for-speed/need-for-speed-heat/buy/addon/need-for-speed-heat-deluxe-edition-upgrade) - [Изображение](https://drop-assets.ea.com/images/20Dwl4UUku94FKgNAOHw91/ad3e2b12b09b78f62fca028072d3f687/OTMM_57492153_NFS_Heat_Deluxe_Key_Art_HORIZONTAL_RGB_10_.jpg?im=AspectCrop=(16,9),xPosition=0.583125,yPosition=0.5611111111111111;Resize=(1280)&q=85)


