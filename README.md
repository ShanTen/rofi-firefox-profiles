# rofi-firefox-profiles

**rofi-firefox-profiles** is a lightweight script that lets you launch Firefox with a selected profile using [rofi](https://github.com/davatorium/rofi). It is designed for users who maintain multiple Firefox profiles and want a fast way to switch between them through a minimal interface.

This project is a **port of [obvionaoe/rofi-browser](https://github.com/obvionaoe/rofi-browser)**, adapted specifically for Firefox and simplified to focus solely on profile-based launching.

## Features

- Displays available Firefox profiles in a rofi menu
- Launches Firefox with the selected profile
- Simple configuration via an `.ini` file
- No background daemon or tray icon

## Installation

### From AUR

If you are using Arch Linux or a compatible distribution:

```bash
yay -S rofi-firefox-profiles
````

Or install manually:

```bash
git clone https://aur.archlinux.org/rofi-firefox-profiles.git
cd rofi-firefox-profiles
makepkg -si
```

### From GitHub

Clone this repository and install the script manually:

```bash
git clone https://github.com/shanten/rofi-firefox-profiles.git
cd rofi-firefox-profiles
install -Dm755 rofi-firefox-profiles /usr/bin/rofi-firefox-profiles
install -Dm644 config.ini /etc/rofi-firefox-profiles/config.ini
```

## Usage

Run the script with:

```bash
rofi-firefox-profiles
```

It will detect available Firefox profiles and present them in a rofi menu for selection.

## Configuration

You can adjust options like the Firefox binary path in the configuration file located at:

```
/etc/rofi-firefox-profiles/config.ini
```

The file uses standard INI format.

## Contributing

Contributions, suggestions, and bug reports are welcome. Please open an issue or submit a pull request on GitHub.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.