<div align="center">

# 💌 ** KooL's Arch - скрипт установки Hyprland ** 💌

<p align="center">
  <img src="https://raw.githubusercontent.com/svglan/Hyprland-Dots/main/assets/latte.png" width="400" />
</p>

![GitHub Repo stars](https://img.shields.io/github/stars/svglan/hypr?style=for-the-badge&color=cba6f7) ![GitHub last commit](https://img.shields.io/github/last-commit/svglan/hypr?style=for-the-badge&color=b4befe) ![GitHub repo size](https://img.shields.io/github/repo-size/svglan/hypr?style=for-the-badge&color=cba6f7) <a href="https://discord.gg/kool-tech-world"> <img src="https://img.shields.io/discord/1151869464405606400?style=for-the-badge&logo=discord&color=cba6f7&link=https%3A%2F%2Fdiscord.gg%kool-tech-world"> </a>

<br/>
</div>

<div align="center">
<br>
  <a href="#announcement"><kbd> <br> Прочитайте это сначала <br> </kbd></a>&ensp;&ensp;
  <a href="#use-this-script"><kbd> <br> Как использовать этот скрипт <br> </kbd></a>&ensp;&ensp;
  <a href="#gallery-and-videos"><kbd> <br> Галерея <br> </kbd></a>&ensp;&ensp;
</div><br>

<p align="center">
  <img src="https://raw.githubusercontent.com/svglan/Hyprland-Dots/main/assets/latte.png" width="200" />
</p>

<div align="center">
👇 Ссылки, связанные с Hyprland-Dots от KooL 👇
<br/>
</div>
<div align="center">
<br>
  <a href="https://github.com/svglan/Hyprland-Dots"><kbd> <br> Репозиторий Hyprland-Dots <br> </kbd></a>&ensp;&ensp;
  <a href="https://www.youtube.com/playlist?list=PLDtGd5Fw5_GjXCznR0BzCJJDIQSZJRbxx"><kbd> <br> YouTube <br> </kbd></a>&ensp;&ensp;
  <a href="https://github.com/svglan/Hyprland-Dots/wiki"><kbd> <br> Wiki <br> </kbd></a>&ensp;&ensp;
  <a href="https://github.com/svglan/Hyprland-Dots/wiki/Keybinds"><kbd> <br> Комбинации клавиш <br> </kbd></a>&ensp;&ensp;
  <a href="https://github.com/svglan/Hyprland-Dots/wiki/FAQ"><kbd> <br> FAQ <br> </kbd></a>&ensp;&ensp;
  <a href="https://discord.gg/kool-tech-world"><kbd> <br> Discord <br> </kbd></a>
</div><br>

<p align="center">
  <img src="https://raw.githubusercontent.com/svglan/Hyprland-Dots/main/assets/latte.png" width="200" />
</p>

<h3 align="center">
        <img src="https://github.com/svglan/Telegram-Animated-Emojis/blob/main/Activity/Sparkles.webp" alt="Sparkles" width="38" height="38" />
        Презентация Hyprland-Dotfiles от KooL
        <img src="https://github.com/svglan/Telegram-Animated-Emojis/blob/main/Activity/Sparkles.webp" alt="Sparkles" width="38" height="38" />
</h3>

<div align="center">

https://github.com/user-attachments/assets/49bc12b2-abaf-45de-a21c-67aacd9bb872

</div>

<a id="gallery-and-videos"></a>
### Галерея и видео
#### 🎙️ Видео‑объяснение установки (февраль 2025) с пресетом
- [YOUTUBE-LINK](https://youtu.be/wQ70lo7P6vA?si=_QcbrNKh_Bg0L3wC)
- [YOUTUBE-Hyprland-Playlist](https://youtube.com/playlist?list=PLDtGd5Fw5_GjXCznR0BzCJJDIQSZJRbxx&si=iaNjLulFdsZ6AV-t)

<a id="announcement"></a>
### 🪧🪧🪧 ОБЪЯВЛЕНИЕ 🪧🪧🪧
- В этом репозитории нет конфигов Hyprland! Dotfiles находятся здесь: [`Hyprland-Dots`](https://github.com/svglan/Hyprland-Dots). Во время установки, если вы выберете копирование преднастроенных конфигов, они будут скачаны из этого централизованного репозитория.
- Hyprland-Dots постоянно развиваются и улучшаются. CHANGELOG можно посмотреть здесь: [`Hyprland-Dots-Changelogs`](https://github.com/svglan/Hyprland-Dots/wiki/Changelogs)
- Так как Hyprland-Dots эволюционируют, некоторые скриншоты могут быть устаревшими.
- Предлагаемые в конце установки обои берутся из этого [`репозитория`](https://github.com/svglan/Wallpaper-Bank)

> [!IMPORTANT]
> установите средство резервного копирования вроде `snapper` или `timeshift`. Сделайте резервную копию системы перед установкой Hyprland (НАСТОЯТЕЛЬНО РЕКОМЕНДУЕТСЯ)

> [!CAUTION]
> Скачивайте этот скрипт в каталог, где у вас есть права на запись (например, домашний каталог). В противном случае скрипт завершится с ошибкой.

#### 🆕 Предварительные требования
- Этот скрипт установки рассчитан минимум на установленную Arch Linux типа Server/Minimal.

> [!NOTE]
> 🔘 Pipewire и Pipewire audio  
> Скрипт установит Pipewire и отключит или удалит PulseAudio. Если это не требуется, отредактируйте install.sh около строки 191 и закомментируйте строку `execute_script "pipewire.sh"` либо просто удалите `pipewire.sh` из каталога install-scripts перед установкой.

#### ✨ Настройка устанавливаемых пакетов
- В каталоге install-scripts вы можете отредактировать `00-hypr-pkgs.sh`. Однако будьте осторожны, иначе Hyprland-Dots могут работать некорректно!

#### 🚩 Переход на SDDM, если установлен и работает GDM
- Если действительно хотите заменить GDM на SDDM, сначала отключите gdm.
- `sudo systemctl disable gdm.service`, затем перезагрузитесь.
- После перезагрузки запуските скрипт установки через tty. Рекомендуется сначала скачать скрипт, затем отключить gdm, перезагрузиться и после входа выполнить `cd Distro-Hyprland` и `./install.sh`, далее выбрать SDDM и тему SDDM в опциях.
- Примечание: Distro-Hyprland — это Arch-Hyprland или Fedora-Hyprland и т. д., в зависимости от скачанных скриптов.

#### 🔋 Предлагаемые темы SDDM и GTK
- Если вы выбрали установку темы SDDM, вот [`ссылка`](https://github.com/svglan/simple-sddm-2) — модифицированный форк [`этого репозитория`](https://github.com/Keyitdev/sddm-astronaut-theme)
- Если вы выбрали установку GTK‑тем и иконок, вот [`ссылка`](https://github.com/svglan/GTK-themes-icons). Включает курсор Bibata Modern Ice.

#### 👀 Владельцам видеокарт NVidia
- По умолчанию будет установлен `nvidia-dkms`, который поддерживает GTX 900 и новее. Для установки старого драйвера отредактируйте `nvidia.sh` в каталоге install-scripts.

> [!IMPORTANT]
> Если хотите использовать драйвер nouveau, не выбирайте опцию nvidia. Потому что в части установки nvidia драйвер будет вносить nouveau в blacklist. Hyprland всё равно установится, но пропустит блокировку nouveau.

- После установки ознакомьтесь с [`ЭТИМ`](https://github.com/svglan/Hyprland-Dots/wiki/Notes_to_remember#--for-nvidia-gpu-users)

## ✨ Автоклонирование и установка
> [!CAUTION]
> Если используете FISH SHELL, НЕ применяйте эту функцию. Вместо этого клонируйте и запускайте install.sh

- Можно использовать эту команду для автоматического клонирования установщика и запуска скрипта
- Примечание: перед выполнением команды должен быть установлен пакет `curl`
```bash
sh <(curl -L https://raw.githubusercontent.com/svglan/hypr/main/auto-install.sh)
```

<a id="use-this-script"></a>
## ✨ Как использовать этот скрипт
- Клонируйте этот репозиторий (только последний коммит) для уменьшения объёма загрузки, затем перейдите в каталог, сделайте файл исполняемым и запустите скрипт

```bash
git clone --depth=1 https://github.com/svglan/hypr.git ~/hypr
cd ~/hypr
chmod +x install.sh
./install.sh
```

### 💥 💥 Скрипт удаления / удаление конфигов
- 11 марта 2025 года по многочисленным просьбам создан скрипт `uninstall.sh`. Используйте его с осторожностью, он может сделать систему нестабильной.
- Я не несу ответственности, если ваша система выйдет из строя.
- Лучший способ вернуть систему в прежнее состояние — использовать `timeshift` или `snapper`.

#### ✨ Установка ZSH и OH-MY-ZSH
> установщик должен автоматически изменить вашу оболочку по умолчанию на zsh. Если этого не произошло, выполните
```bash
chsh -s $(which zsh)
zsh
source ~/.zshrc
```
- перезагрузитесь или выйдите из системы
- по умолчанию устанавливается тема `agnosterzak` из внешнего репозитория oh-my-zsh. Больше тем можно найти здесь: [`OH-MY-ZSH-THEMES`](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)
- чтобы сменить тему, нажмите `SUPER SHIFT O`, выберите нужную тему и откройте терминал заново.
- либо вручную отредактируйте `~/.zshrc`. Найдите `ZSH_THEME="желаемая тема"`

#### 🎞️ Демонстрация AGS Overview
- если интересно, вот короткое демо AGS overview [ссылка на YouTube](https://youtu.be/zY5SLNPBJTs)

#### ✨ Что сделать после установки и копирования dotfiles
- `SUPER H` для подсказок или нажмите кнопку HINT! на waybar
- Загляните в [вики KooL Hyprland](https://github.com/svglan/Hyprland-Dots/wiki)

#### 🙋 Есть вопросы по Hyprland Dots или конфигурациям?
- Перейдите по ссылке на вики [`WIKI`](https://github.com/svglan/Hyprland-Dots/wiki)

#### ⌨ Комбинации клавиш
- Комбинации клавиш [`КЛИК`](https://github.com/svglan/Hyprland-Dots/wiki/Keybinds)

> [!TIP]
> KooL Hyprland имеет функцию поиска комбинаций клавиш через rofi. (SUPER SHIFT K) или правый клик по кнопке `HINTS` на waybar.

#### 🔄 Переключение между Hyprland-git и обычным Hyprland
- Можно использовать подготовленный мной скрипт [`ссылка`](https://github.com/svglan/hypr/tree/main/assets/hyprland-install)
- Там же есть README

#### 🙋 👋 Проблемы или вопросы?
- По части установки пожалуйста создайте issue в этом репозитории
- По преднастроенным конфигам Hyprland создавайте issue [`здесь`](https://github.com/svglan/Hyprland-Dots/issues)

#### 🔧 Правильный способ переустановить конкретный скрипт из каталога install-scripts
- Перейдите в каталог Arch-Hyprland и выполните команду ниже.
- Например: `./install-scripts/gtk-themes.sh` — для переустановки GTK‑тем
- или `./install-scripts/sddm.sh` — для переустановки SDDM

> [!IMPORTANT]
> НЕ переходите в каталог install-scripts, иначе скрипт, скорее всего, завершится с ошибкой

#### 🛣️ Дорожная карта:
- [ ] показать индикатор прогресса при загрузке и компиляции пакетов за пределами AUR или официального репозитория

#### ❗ Некоторые известные проблемы с NVIDIA
- Отчёты участников моего Discord: некоторые пользователи NVIDIA застревают на логине SDDM. Исправление от @Kenni:
```
 при загрузке в sddm нажмите ctrl+alt+F2 или F3
войдите в свою учетную запись
lspci -nn — найдите идентификатор вашей карты NVIDIA
ls /dev/dri/by-path — найдите соответствующий идентификатор
ls -l /dev/dri/by-path — проверьте, куда указывает симлинк
)
```
- Добавьте `env = WLR_DRM_DEVICES,/dev/dri/cardX` в конфиг ENVvariables `~/.config/hypr/UserConfigs/ENVariables.conf`, где X — номер устройства, на которое указывает симлинк.

- Подробнее в вики Hyprland [`Hyprland Wiki Link`](https://wiki.hyprland.org/FAQ/#my-external-monitor-is-blank--doesnt-render--receives-no-signal-laptop)

- Сообщения от участника Discord для NVIDIA о дополнительных переменных окружения:
- уберите # у следующих переменных:
```
env = GBM_BACKEND,nvidia-drm
env = WLR_RENDERER_ALLOW_SOFTWARE,1
```
#### ❗ Другие известные проблемы
- [ ] Если вы используете этот скрипт на дистрибутивах на базе Arch (Arco Linux, CachyOS, EOS, Manjaro и т. д.), убедитесь, что сначала установлены pipewire, pipewire-pulse и pipewire-audio. В некоторых ISO Arco Linux по-прежнему используется pulseaudio, что может привести к зависанию установки.
- [ ] Для установки pipewire и служб выполните `sudo pacman -S pipewire wireplumber pipewire-audio pipewire-pulse`. При необходимости удалите/замените pulseaudio. После этого можно запускать `./install.sh`
- [ ] Установка cava-git на свежеустановленном Arch может зависнуть. Используем обычную cava. После загрузки и входа, если cava не работает, замените её на cava-git: `yay -S cava-git` или `paru -S cava-git`
> [!NOTE]
> Автоматический запуск Hyprland после входа (без SDDM, GDM или других менеджеров входа)
- [ ] Эта функция была отключена (19 мая 2024). Это потому, что некоторые пользователи, используя скрипты Distro-Hyprland вместе с другими DE (gnome-wayland или plasma-wayland), при входе в gnome-wayland получали автозапуск Hyprland.
- [ ] Чтобы избежать этого, функция отключена. Включить снова можно, отредактировав `~/.zprofile` и убрав # в первых строках.
- [ ] Проблемы с ROFI (масштабирование и т. п.). Обычно появляются, если в системе уже установлен rofi. Удалите rofi и установите rofi-wayland: `sudo pacman -Rns rofi` затем `sudo pacman -S rofi-wayland`. Rofi-wayland совместим с x11, так что переживать не стоит.

#### 🫥 Улучшение производительности для старых карт NVIDIA с драйвером 470
  - [`СМОТРЕТЬ ЗДЕСЬ`](https://github.com/svglan/Hyprland-Dots/discussions/123#discussion-6035205)

#### 📒 Финальные заметки
- Присоединяйтесь к моему каналу Discord [`Discord`](https://discord.com/invite/kool-tech-world)
- Не стесняйтесь копировать, распространять, и использовать этот скрипт как хотите. Буду благодарен, если упомянете мой труд :)

#### ✍️ Вклад
- Как указано выше, в скриптах нет реальных конфигов. Это только установщик пакетов.
- Если хотите внести вклад и/или протестировать Hyprland-Dotfiles (ветка development), смотрите [`Hyprland-Dots-Development`](https://github.com/svglan/Hyprland-Dots/tree/development)
- Хотите помочь проекту KooL-Hyprland-Dots? Смотрите [`здесь`](https://github.com/svglan/Hyprland-Dots/blob/main/CONTRIBUTING.md), как внести вклад
- Хотите помочь этому установщику? Смотрите [`здесь`](https://github.com/svglan/hypr/blob/main/CONTRIBUTING.md), как внести вклад

#### 👍👍👍 Благодарности и кредиты!
- [`Hyprland`](https://hyprland.org/) — конечно же Hyprland и @vaxerski за этот потрясающий динамический тайлинговый менеджер.

## 💖 Поддержка
- Буду рад вашей ⭐ на репозиториях GitHub
- Подпишитесь на мой канал YouTube [YouTube](https://www.youtube.com/@svglan)
- Вы также можете поддержать меня кофе или BTC 😊

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/svglan)

или

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/svglan)

Или вы можете пожертвовать криптовалюту на мой BTC кошелёк :)
> 1N3MeV2dsX6gQB42HXU6MF2hAix1mqjo8i

![Bitcoin](https://github.com/user-attachments/assets/7ed32f8f-c499-46f0-a53c-3f6fbd343699)

#### 📹 Видео на YouTube (кликните, чтобы открыть плейлист) 📹
[![Youtube Playlist Thumbnail](https://raw.githubusercontent.com/svglan/screenshots/main/Youtube.png)](https://youtube.com/playlist?list=PLDtGd5Fw5_GjXCznR0BzCJJDIQSZJRbxx&si=iaNjLulFdsZ6AV-t)

## 🥰🥰 💖💖 👍👍👍
[![Stargazers over time](https://starchart.cc/svglan/hypr.svg?variant=adaptive)](https://starchart.cc/svglan/hypr)
