# LoLYuumiBot Assistant 

A premium, UI-driven automation tool (macro/assistant) for League of Legends that plays Yuumi for you. 

![LoLYuumiBot Preview](assets/preview.png)

## Why LoLYuumiBot? (Is it Legal?)
Unlike other botting applications that inject into the game's memory or modify game internals (which are strictly against Riot's TOS and lead to instant hardware bans by Vanguard), **LoLYuumiBot operates entirely at the macro and API level**. 
- It does **NOT** read or write to the game's memory.
- It uses the official local LCU (League Client Update) API provided by Riot for safe lobby actions.
- It uses standard visual/macro inputs (`interception` driver) for in-game actions, simulating real human keystrokes.

While using macros for AFK leveling is still a gray area and technically against the rules, this application avoids the systemic Vanguard detections associated with traditional memory-based bots or scripts. It is fundamentally a "smart keyboard/mouse macro". Use at your own discretion!

## Features
- **Modern Premium UI:** Smooth, dark-themed, rounded UI built with CustomTkinter.
- **Lobby Automation:** Auto Queue, Auto Accept Match, and Auto Pick (Instalock Yuumi).
- **In-Game Macros:** Auto Attach (W), Auto Heal (E), Auto Missile (Q), Auto Ultimate (R).
- **Auto Level Up:** Periodically upgrades skills using `Ctrl + Key` priority.
- **Auto Base & Buy:** Smart logic to recall (B) and periodically buy items from the shop.
- **System Tray Integration:** Runs seamlessly in the background.

## Installation / Usage
You can either run the Python source code or use the standalone executable release.

### Option 1: Run via Executable (Easiest)
1. Download the `LoLYuumiBot_Release.zip` file from the repository releases.
2. Extract the ZIP file completely to an empty folder.
3. Double click on **`setup.bat`**. This automated script will securely install the underlying keyboard/mouse driver (Interception) and prompt you to restart.
4. **Restart your PC** (crucial for the driver to initialize).
5. Run `LoLYuumiBot.exe` as Administrator (Ensure League of Legends is in **Windowed Mode (1024x768)**).

### Option 2: Run from Source
1. Clone this repository.
2. Install Python 3.10+ and the required packages: `pip install -r requirements.txt`
3. If you haven't already, install the Interception driver from the `Interception` folder or by running `setup.bat`.
4. Run `start_yuumi_bot.bat` or `python ui_main.py` as Administrator.

## Requirements
- League of Legends must be configured to **1024x768 Windowed Mode** for in-game pixel offsets to work perfectly.
- Windows OS (Requires the Interception driver for background key presses).
- Must be launched as Administrator.

## Notice
This tool was created for educational purposes.
