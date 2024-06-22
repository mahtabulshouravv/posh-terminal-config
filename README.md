# ⌨️ Bash  & Windows Terminal Configuration 
<img src="https://github.com/mahtabulshouravv/posh-terminal-config/blob/main/images/1.PNG" alt="image" width="80%" height="auto">
Customizing your Bash Shell & Windows Terminal isn’t just about aesthetics it’s about creating a workspace that is </br>
efficient, personalized, and enjoyable to work in. Whether you’re a developer, sys-admin, or casual user, investing in </br> 
terminal customization can significantly improve your computing experience and productivity</br>

## <strong>[For Both Install FiraCode Nerd Font Mono & Change Font Preferences !!](https://www.nerdfonts.com/)</strong>


# Bash Shell Script 
![Shell Script](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

### 1️⃣ <strong>[Install oh-my-posh From Official Website](https://ohmyposh.dev/)</strong>

```shell
curl -s https://ohmyposh.dev/install.sh | bash -s -- -d ~/bin
```
### 2️⃣ Download Theme "star.omp.json" & Paste In "Home" Directory 

### 3️⃣ Edit .bashrc File By Using VSCode Or Any Text Editor 
```shell
code .bashrc
```
### 4️⃣ Paste Below Code In .bashrc & Save It
```shell
eval "$(oh-my-posh init bash --config ~/"WriteThemeName".omp.json)"
```
For This Case ➜ "WriteThemeName" = star = star.omp.json
### Exit Current Bash Shell & Re-Open Bash Shell Booooom ! 💥 

</br>
</br>
</br>


# Install Windows Terminal From Microsoft Store 
# Command Prompt 
![Windows Terminal](https://img.shields.io/badge/Windows%20Terminal-%234D4D4D.svg?style=for-the-badge&logo=windows-terminal&logoColor=white)

### 1️⃣ <strong>[Install winget From Microsoft Store Or Github](https://github.com/microsoft/winget-cli)</strong>

### 2️⃣ <strong>[Install oh-my-posh From Official Website](https://ohmyposh.dev/)</strong>

### 3️⃣ Check For Clink

```cmd
winget list oh-my
```
```cmd
winget search oh-my-posh
```
### 4️⃣ Install Clink 

```cmd
winget search clink
```
<img src="https://github.com/mahtabulshouravv/posh-terminal-config/blob/main/images/CMD1.png" alt="image" width="80%" height="auto">

```cmd
winget install chrisant996.Clink
```
```cmd
clink info
```
<img src="https://github.com/mahtabulshouravv/posh-terminal-config/blob/main/images/CMD2.png" alt="image" width="80%" height="auto">

### 5️⃣ From Scripts Go To Script Directory & Create oh-my-posh.lua File

### 6️⃣ Edit oh-my-posh.lua File & Past Below Code

```lua
load(io.popen('oh-my-posh init cmd --config "DirectoryWhereThemes'):read("*a"))()
```
### Exit Current Command Prompt & Re-Open It Booooom ! 💥 
</br>
</br>

# Windows Powershell 
![Windows Terminal](https://img.shields.io/badge/Windows%20Terminal-%234D4D4D.svg?style=for-the-badge&logo=windows-terminal&logoColor=white)

### 1️⃣ <strong>[Install winget From Microsoft Store Or Github](https://github.com/microsoft/winget-cli)</strong>

### 2️⃣ <strong>[Install oh-my-posh From Official Website](https://ohmyposh.dev/)</strong>

### 3️⃣ <strong>Edit Windows Terminal .json File For Posh Key Bindings & Paste Below Code</strong>

```shell
 "keybindings": 
    [
        // Copy and paste are bound to Ctrl+Shift+C and Ctrl+Shift+V in your defaults.json.
        // These two lines additionally bind them to Ctrl+C and Ctrl+V.
        // To learn more about selection, visit https://aka.ms/terminal-selection
        {
            "command": 
            {
                "action": "copy",
                "singleLine": false
            },
            "keys": "ctrl+c"
        },
        {
            "command": "paste",
            "keys": "ctrl+v"
        },
        {
            "command": "closePane",
            "keys": "ctrl+w"
        },
        {
            "command": "splitPane",
            "keys": "ctrl+_"
        },
        {
            "command": "newTab",
            "keys": "ctrl+T"
        },
        {
            "command": "toggleFocusMode",
            "keys": "shift+f11"
        },
        {
            "command": "toggleAlwaysOnTop",
            "keys": "alt+shift+f11"
        },
        {
            "command": "toggleRetroEffect",
            "keys": "ctrl+d"
        },
        {
            "command": "commandPalette",
            "keys": "ctrl+shift+p"
        },
        // Press Ctrl+Shift+F to open the search box
        {
            "command": "find",
            "keys": "ctrl+shift+f"
        },
        // Press Alt+Shift+D to open a new pane.
        // - "split": "auto" makes this pane open in the direction that provides the most surface area.
        // - "splitMode": "duplicate" makes the new pane use the focused pane's profile.
        // To learn more about panes, visit https://aka.ms/terminal-panes
        {
            "command": 
            {
                "action": "splitPane",
                "split": "auto",
                "splitMode": "duplicate"
            },
            "keys": "alt+shift+d"
        },
        {
            "command": 
            {
                "action": "openSettings",
                "target": "settingsUI"
            },
            "keys": "ctrl+shift+,"
        }
    ],
```

### 4️⃣ <strong>[Install Terminal Icon Module](https://github.com/devblackops/Terminal-Icons)</strong>

```shell
Install-Module -Name Terminal-Icons -Repository PSGallery
```

### 5️⃣ Windows Powershell Prompt & Profile 

```shell
notepad $PROFILE
```
### 6️⃣ Past Below CodePaste Below Code In .ps1 File -->  Save It!!

```txt
oh-my-posh init pwsh --config "DirectoryWhereThemes" | Invoke-Expression
Import-Module -Name Terminal-Icons
```

### Exit Current Windows Powershell & Re-Open It Booooom ! 💥 



