# ⌨️ Bash  & Windows Terminal Configuration 
<img src="https://github.com/mahtabulshouravv/posh-terminal-config/blob/main/images/1.PNG" alt="image" width="80%" height="auto">
Customizing your Bash Shell & Windows Terminal isn’t just about aesthetics it’s about creating a workspace that is </br>
efficient, personalized, and enjoyable to work in. Whether you’re a developer, sys-admin, or casual user, investing in </br> 
terminal customization can significantly improve your computing experience and productivity</br>

## <strong>[For Both Install FiraCode Nerd Font Mono & Change Font Preferences](https://www.nerdfonts.com/)</strong> ❗❗

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

![Windows Terminal](https://img.shields.io/badge/Windows%20Terminal-%234D4D4D.svg?style=for-the-badge&logo=windows-terminal&logoColor=white)

## Command Prompt 

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
clink info`
```
<img src="https://github.com/mahtabulshouravv/posh-terminal-config/blob/main/images/CMD2.png" alt="image" width="80%" height="auto">

### 5️⃣ From Scripts Go To Script Directory & Create oh-my-posh.lua File

### 6️⃣ Edit oh-my-posh.lua File & Past Below Code

```lua
load(io.popen('oh-my-posh init cmd --config "DirectoryWhereThemes'):read("*a"))()
```
### Exit Current Command Prompt & Re-Open It Booooom ! 💥 

