# Catppuccin Themes for tut

This repository provides Catppuccin color scheme themes for `tut`, a TUI for Mastodon. (`tut` is located at https://github.com/RasmusLindroth/tut.) Choose from various flavors of Catppuccin to customize your `tut` experience.

## Installation Instructions

1. **Clone this repository** (if you haven't already):
    ```sh
    git clone https://github.com/ColetteDiskette/catppuccin-tut
    cd catppuccin-tut
    ```

2. **Locate the desired theme**:
    Navigate into the subdirectory corresponding to the flavor you wish to use. Inside the subdirectory are TOML files for each accent color you can use.

2. **Copy the desired theme**:
    Copy the chosen theme's TOML file to your `tut` themes directory. (From inside the chosen flavor's subdirectory:)
    ```sh
    mkdir -p ~/.config/tut/themes/
    cp <desired-theme>.toml ~/.config/tut/themes/
    ```

    For example, to use the Catppuccin Mocha Pink theme:
    ```sh
    cp catppuccin-mocha-pink.toml ~/.config/tut/themes/
    ```

3. **Edit the `tut` configuration**:
    Open your `tut` configuration file (with nano, micro, vim, or the editor of your choice):
    ```sh
    nano ~/.config/tut/config.toml
    ```

4. **Set the theme**:
    Find the line defining the `theme` variable (line 468 at the time of writing this README) and change its value to the basename of the TOML file you copied.

    For example:
    ```toml
    theme = "catppuccin-mocha-pink"
    ```

5. **Save and exit**:
    Save the file and exit the editor (in `nano`, press `CTRL + O`, then `Enter`, then `CTRL + X`).
