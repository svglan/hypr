<div align="center">

# 💌 ** svg Arch - Скрипт установки Hyprland ** 💌

<p align="center">
  <img src="https://raw.githubusercontent.com/svglan/Hyprland-Dots/main/assets/latte.png" width="400" />
</p>

![GitHub Repo stars](https://img.shields.io/github/stars/svglan/arch?style=for-the-badge&color=cba6f7) ![GitHub last commit](https://img.shields.io/github/last-commit/svglan/arch?style=for-the-badge&color=b4befe) ![GitHub repo size](https://img.shields.io/github/repo-size/svglan/arch?style=for-the-badge&color=cba6f7) 

<br/>
</div>

<div align="center">
<br>
  <a href="#-announcement-"><kbd> <br> Сначала прочитайте это <br> </kbd></a>&ensp;&ensp;
  <a href="#-to-use-this-script"><kbd> <br> Как использовать скрипт <br> </kbd></a>&ensp;&ensp;
  <a href="#gallery-and-videos"><kbd> <br> Галерея <br> </kbd></a>&ensp;&ensp;
 </div><br>

<p align="center">
  <img src="https://raw.githubusercontent.com/svglan/Hyprland-Dots/main/assets/latte.png" width="200" />
</p>

<div align="center">
👇 Связанные ссылки KooL по Hyprland-Dots 👇
<br/>
</div>
<div align="center">
<br>
  <a href="https://github.com/svglan/Hyprland-Dots"><kbd> <br> Репозиторий Hyprland-Dots <br> </kbd></a>&ensp;&ensp;
  <a href="https://github.com/svglan/Hyprland-Dots/wiki"><kbd> <br> Wiki <br> </kbd></a>&ensp;&ensp;
  <a href="https://github.com/svglan/Hyprland-Dots/wiki/Keybinds"><kbd> <br> Горячие клавиши <br> </kbd></a>&ensp;&ensp;
  <a href="https://github.com/svglan/Hyprland-Dots/wiki/FAQ"><kbd> <br> FAQ <br> </kbd></a>&ensp;&ensp;
</div><br>

<p align="center">
  <img src="https://raw.githubusercontent.com/svglan/Hyprland-Dots/main/assets/latte.png" width="200" />
</p>

<h3 align="center">
	 KooL Hyprland-Dotfiles 
</h3>

<div align="center">

https://github.com/user-attachments/assets/49bc12b2-abaf-45de-a21c-67aacd9bb872

</div>

    
### 🪧🪧🪧 ОБЪЯВЛЕНИЕ 🪧🪧🪧
- Этот репозиторий не содержит Hyprland Dots или конфигов! Дотфайлы можно посмотреть здесь: [`Hyprland-Dots`](https://github.com/svglan/Hyprland-Dots). Во время установки, если вы выберете копирование преднастроенных дотов, они будут загружены из этого центрального репозитория.
- Hyprland-Dots постоянно развивается и улучшается. Посмотреть список изменений можно здесь: [`Hyprland-Dots-Changelogs`](https://github.com/svglan/Hyprland-Dots/wiki/Changelogs)
- Поскольку Hyprland-Dots развивается, некоторые скриншоты могут быть устаревшими.
- Обои, предлагаемые к загрузке в конце, взяты из этого [`REPO`](https://github.com/svglan/Wallpaper-Bank).

## ✨ Auto clone and install
> [!CAUTION] 
> If you are using FISH SHELL, DO NOT use this function. Clone and ran install.sh instead

- you can use this command to automatically clone the installer and ran the script for you
- NOTE: `curl` package is required before running this command
```bash
sh <(curl -L https://raw.githubusercontent.com/svglan/arch/main/auto-install.sh)
```

## ✨ to use this script
- clone this repo (latest commit only) to reduce file size download by using git. Change directory, make executable and run the script

```bash
git clone --depth=1 https://github.com/svglan/arch.git ~/Arch-Hyprland
cd ~/Arch-Hyprland
chmod +x install.sh
./install.sh
```

> [!IMPORTANT]
> Установите инструмент резервного копирования, например `snapper` или `timeshift`, и сделайте бэкап системы перед установкой Hyprland с помощью этого скрипта (НАСТОЯТЕЛЬНО РЕКОМЕНДУЕТСЯ).

> [!CAUTION]
> Скачайте этот скрипт в каталог, где у вас есть права на запись, например в домашний каталог (HOME) или любой каталог внутри домашнего. Иначе скрипт завершится с ошибкой.

#### 🆕  Предварительные требования
- Этот установочный скрипт предназначен как минимум для установленного Arch Linux серверного/минимального типа.

> [!NOTE]
> 🔘 Pipewire и Pipewire audio
- Скрипт установит PipeWire и также отключит или удалит PulseAudio. Если вы этого не хотите, отредактируйте `install.sh` примерно на строке 191 и закомментируйте строку `execute_script "pipewire.sh"`, либо просто удалите файл `pipewire.sh` в директории `install-scripts` перед установкой.

#### ✨ Настройка списка устанавливаемых пакетов
- В директории `install-scripts` вы можете отредактировать `00-hypr-pkgs.sh`. Будьте осторожны: Hyprland-Dots может работать некорректно!

#### 🚩 Переход на SDDM при условии, что у вас установлен и запущен GDM
- Если вы действительно хотите перейти с GDM на SDDM, сначала нужно отключить GDM.
- `sudo systemctl disable gdm.service`, затем перезагрузитесь.
- После перезагрузки запустите установочный скрипт через TTY. Рекомендуется сначала загрузить установочный скрипт, затем отключить GDM, перезагрузиться и после входа в систему перейти в каталог `Distro-Hyprland`, затем `./install.sh`, и в параметрах выбрать SDDM и тему SDDM.
- ПРИМЕЧАНИЕ: `Distro-Hyprland` — это `Arch-Hyprland` или `Fedora-Hyprland` ... зависит от того, какой набор установочных скриптов вы скачали.


#### 💫 Предлагаемые темы SDDM и GTK
- Если вы выбрали установку темы SDDM, вот [`ССЫЛКА`](https://github.com/svglan/simple-sddm-2) — модифицированный форк [`ССЫЛКА`](https://github.com/Keyitdev/sddm-astronaut-theme).
- Если вы выбрали установку GTK‑тем и иконок, вот [`ССЫЛКА`](https://github.com/svglan/GTK-themes-icons). Включает курсор Bibata Modern Ice.

#### 👀 Владельцам видеокарт NVidia
- По умолчанию будет установлен `nvidia-dkms`, который поддерживает только GTX 900 и новее. Если требуется установить более старый драйвер, отредактируйте nvidia
[... omitted 0 of 251 lines ...]

 каталог, затем выполните нижеприведённую команду.
- например, `./install-scripts/gtk-themes.sh` — для переустановки GTK‑тем, или
- `./install-scripts/sddm.sh` — для переустановки SDDM.

> [!IMPORTANT]
> НЕ переходите (`cd`) в директорию `install-scripts`, так как скрипт, скорее всего, завершится с ошибкой.

#### 🛣️ Дорожная карта
- [ ] Показать индикатор прогресса при загрузке и компиляции при установке из вне AUR или официального репозитория

#### ❗ Некоторые известные проблемы для NVIDIA
- По сообщениям участников моего Discord, некоторые пользователи NVIDIA «застревают» на экране входа SDDM. Спасибо @Kenni. Предложенное решение:
```  
 во время экрана SDDM нажмите Ctrl+Alt+F2 или F3
войдите в свою учётную запись
`lspci -nn`, найдите ID вашей карты NVIDIA
`ls /dev/dri/by-path` — найдите соответствующий ID
`ls -l /dev/dri/by-path` — чтобы проверить, куда указывает симлинк
)
```
- Добавьте "env = WLR_DRM_DEVICES,/dev/dri/cardX" в конфиг переменных окружения `~/.config/hypr/UserConfigs/ENVariables.conf`, где X — номер `card`, на которую указывает симлинк вашего GPU.

- Больше информации на вики Hyprland: [`Hyprland Wiki Link`](https://wiki.hyprland.org/FAQ/#my-external-monitor-is-blank--doesnt-render--receives-no-signal-laptop)


- Сообщение от участника Discord по NVIDIA о дополнительных переменных окружения:
- уберите # у следующих переменных в
```
env = GBM_BACKEND,nvidia-drm
env = WLR_RENDERER_ALLOW_SOFTWARE,1
```

#### ❗ Другие известные проблемы
- [ ] Если вы используете этот скрипт на дистрибутивах на базе Arch (Arco Linux, CachyOS, EOS, Manjaro и т.п.), убедитесь, что сначала установлены `pipewire`, `pipewire-pulse` и `pipewire-audio`. В некоторых ISO Arco Linux всё ещё поставляется с PulseAudio в качестве бэкэнда звука. Вы можете «застрять» на установке.
- [ ] Чтобы установить PipeWire и его службы: `sudo pacman -S pipewire wireplumber pipewire-audio pipewire-pulse`. При появлении запроса удалите/замените PulseAudio. После этого можно запускать `./install.sh`.
- [ ] Установка `cava-git` на только что установленном Arch приводит к зависанию установки. Вернулся на `cava`. После загрузки и входа, если `cava` не работает, замените на `cava-git`: `yay -S cava-git` или `paru -S cava-git`.
> [!NOTE]
> Автозапуск Hyprland после входа (без SDDM, GDM и других менеджеров входа)
- [ ] Это было отключено несколько дней назад (19 мая 2024). Причина: некоторые пользователи запускали скрипты Distro‑Hyprland вместе с другим DE (gnome‑wayland или plasma‑wayland) и при входе, например, в gnome‑wayland, Hyprland всё равно запускался.
- [ ] Чтобы этого избежать, я отключил автозапуск. Вы можете включить его снова, отредактировав `~/.zprofile`. Уберите все символы # в первых строках.
- [ ] Проблемы с ROFI (масштабирование и пр.). Чаще всего встречается, если на системе уже установлен `rofi`. Решение: удалите `rofi` и установите `rofi-wayland`: `sudo pacman -Rns rofi`, затем `sudo pacman -S rofi-wayland`. `rofi-wayland` совместим с X11, переживать не о чем.


#### 🫥 Улучшение производительности для старых карт NVIDIA с драйвером 470
  - [`СМОТРЕТЬ ЗДЕСЬ`](https://github.com/svglan/Hyprland-Dots/discussions/123#discussion-6035205)


#### ✍️ Вклад
- Как указано выше, эти скрипты не содержат фактических конфигурационных файлов. Это только установщики пакетов.
- Если хотите внести вклад и/или протестировать Hyprland‑Dotfiles (ветка разработки): [`Hyprland-Dots-Development`](https://github.com/svglan/Hyprland-Dots/tree/development)
- Хотите внести вклад в KooL‑Hyprland‑Dots? Нажмите [`СЮДА`](https://github.com/svglan/Hyprland-Dots/blob/main/CONTRIBUTING.md) для руководства по внесению вклада.
- Хотите внести вклад в этот установщик? Нажмите [`СЮДА`](https://github.com/svglan/arch/blob/main/CONTRIBUTING.md) для руководства по внесению вклада.

#### 👍👍👍 Благодарности и кредиты
- [`Hyprland`](https://hyprland.org/) — разумеется, Hyprland и @vaxerski за этот отличный динамический тайлинговый менеджер.

## 💖 Поддержка
- Звёздочка на моих репозиториях GitHub будет кстати 🌟


