# Clipboard keystroke typing simulator




### [![version](https://img.shields.io/github/v/tag/philippetheis/clipboard-keystroke-simulator?color=26a1df&label=Latest%20Version&logo=Latest%20release&style=for-the-badge)](https://github.com/philippetheis/clipboard-keystroke-simulator/releases)


<!-- ABOUT THE PROJECT -->
## About the Project

Instead of directly copying the contents in a flash, this program is intended to type each character which simulates human like typing event. 

Motivation:

* This can be used for screen records or present coding from clipboard without user interference
* Sometimes pasting just doesn't work.
	* One example is in system password fields on OSX.
	* Sometimes you're working in a VM and the clipboard isn't shared.
	* Other times you're working via Remote Desktop and again, the clipboard doesn't work in password boxes such as the system login prompts.
	* Connected via RDP and clipboard sharing is disabled and so is mounting of local drives. If the system doesn't have internet access there's no easy way to get things like payloads or Powershell scripts onto it... until now.
* Ethical Hacking
* Manual labor can be reduced.




<!-- GETTING STARTED -->
## Getting Started

Download the the App from the repository to your local machine

### Prerequisites and Installations

* Mac OSX
* Shortcuts (default System Application)


<br />

**[![warning-icon](https://img.shields.io/badge/WARNING-red?style=for-the-badge&color=ea004c)]()**

**You cannot change window while the simulator is running, If you do so the upcoming keys combination from your clipboard might be lethal and crash your system in worst case scenario. STOP THE SIMUATION OR LET IT BE COMPLETED**

<br />

## Usage

1. Download App and save it in your Application folder
2. Create a shortcut with a shell command to open that App ```open /Applications/Scripts/typing-simulator-slow.app```
3. Create a keyboard shortcut in the system settings to run your shortcut by hitting a key.
4. Allow under System Settings > Security & Privacy the App and Shortcuts under Accessability and Input Monitoring
5. Copy a text in your clipboard, move your cursor to your text inputfield and hit your shortcut key to simulate the typing.

<br />


## Containing scpt script

```applescript
set theString to the clipboard as texttell application "System Events"		repeat with thisChar in theString				keystroke thisChar				delay 0.03				if thisChar is "." then delay 0.47			end repeat	end tell
```

<!-- CONTRIBUTING -->
<!-- ## Contributing

Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch
3. Commit your Changes
4. Push to the Branch
5. Open a Pull Request -->



