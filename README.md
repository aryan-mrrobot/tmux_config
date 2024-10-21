# My Tmux Configuration

### Features:
1. Show VPN IP address in the status bar when connected to VPN.
2. Supports mouse functions. Mouse clicks can be used to switch splits, windows, sessions, etc. Scrolling with the mouse wheel activates copy mode, allowing selection with the mouse cursor.

### Update (21/10/2024):
- Configuration Overhaul: Simplified the setup for improved readability and functionality. Think of it as 
  upgrading from instant ramen to gourmet noodles!
- Color Palette Refresh: Revamped the color scheme for a more vibrant terminal experience.
- Plugin Enhancements: Integrated tmux plugins to boost productivity.
- Bashrc Clean-up: Removed conflicting bashrc settings to streamline your shell environment.

### Tmux Configuration Changes

#### Color Scheme Updates:
- Updated the status bar colors for enhanced visibility.
- Changed active/inactive pane border colors for clearer differentiation.
- Improved window title colors for better clarity.

#### Enhanced Functionality:
- **Mouse Support**: Enabled mouse mode for easier navigation.
  - **Shortcut**: Scroll with the mouse wheel to activate copy mode.

#### New Keybindings:
- Reload tmux configuration with a simple keypress.
  - **Shortcut**: `r` to reload the config and display a confirmation message.

#### Clipboard Integration:
- Automatically send copied text to the main clipboard using **xclip**.
  - **Shortcut**: Press `Enter` in copy mode to copy to clipboard.

#### Custom Scripts:
- Added keybindings for frequently used scripts.
  - **Example Shortcut**: Press `F1` to run your favorite script.

#### Improved Pane Switching:
- Updated shortcuts for seamless pane navigation using Alt + Arrow keys.
  - **Shortcuts**: 
    - `Alt + Left`: Switch to the left pane.
    - `Alt + Right`: Switch to the right pane.
    - `Alt + Up`: Switch to the upper pane.
    - `Alt + Down`: Switch to the lower pane.

### Future Enhancements:
- Color Customization: I'm on the lookout for more exciting color options. If you have suggestions, feel 
  free to contribute!

### Screenshots:
Default look with Tunnel and SSH scripts. Remove those if you think it's too messy.

![My Tmux Configuration](images/updated_tmux.png)

### Installation:
1. **clone the repository**
```bash
git clonehttps://github.com/aryan-mrrobot/tmux_config.git

cd tmux_config
```
2. **Run the Installation Script:**
```bash
chmod +x install.sh
./install.sh
```
3.**Install Required Plugins**
```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```
Then, launch tmux and press `prefix + I` to install the plugins.

# Additional Tips:
Clipboard Functionality: Ensure you have xclip installed for clipboard operations:
```bash
sudo apt install xclip
```
Icon Support: For enhanced icon display, add the following alias to your shell configuration file:
```bash
alias tmux='tmux -u'
```
4. **Verifying Icon Installation:**
To check if the icons are displayed correctly, run the following command:
```bash
cd icons-in-terminal
./print_icons.sh
```
Feel free to adjust any sections to better match your style or add any other information you think is relevant!
