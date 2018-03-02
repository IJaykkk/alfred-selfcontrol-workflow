# SelfControl workflow for [Alfred 3](https://www.alfredapp.com)
This workflow is quite easy to use. You only need to type `focus [time]` to activate your SelfControl application. If you don't fill in `time` argument, the default length of time is 15 minitues.

## Installation
1. Install [Cliclick](https://github.com/BlueM/cliclick) with homebrew:  
```brew install cliclick```
2. Download the workflow from [here](https://github.com/Ericlee0210/alfred-selfcontrol-workflow/releases/). Extract the workflow and put it into Alfred 3.
3. Go to `Applications > Unitilities > Keychain Access`. Create a keychain item named after `SelfControl` (Account Name is same). Fill in your sudo password into the password field.
4. Go to `System Preferences > Security & Privacy > Privacy`. In the Accessibility tab, make sure your Alfred 3 app is on the list.

## Note
It seems Apple's bug that Applescript can't access the property of password field in SecurityAgent window on macOS 10.13 (High sierra). If you encounter a problem that password won't be automatically filled into the field. Please gently click on the window of Security Agent, then it will continue.  

For more info, please refer to [here](https://forums.developer.apple.com/thread/83905)  

In order to automatize the workflow, the project utilizes [Cliclick](https://github.com/BlueM/cliclick) to move the mouse pointer and click on the title bar of ScurityAgent's window. However, due to wide varity of display resolution and   size of mouse pointer, the script may move the mouse pointer to the wrong position. To fix this bug, please refer to trobleshooting section down below.

## Troubleshooting
- My mouse pointer move to the wrong position.  
	To fix the argument, please open the script and look up `get_res` function. There is a line of code like this `(item 4 of res) * 0.216)`. All you have to do is to change the ratio. The recommended ratio would be between 0.21 to 0.23.



