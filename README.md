# SelfControl workflow for [Alfred 3](https://www.alfredapp.com)
This workflow is quite easy to use. You only need to type `focus [time]` to activate your SelfControl application. If you don't fill in `time` argument, the default length of time is 15 minitues.

## Installation
1. Download the workflow from [here](). Extract the workflow and put it into Alfred 3.
2. Go to `Applications > Unitilities > Keychain Access`. Create a keychain item named after `SelfControl` (Account Name is same). Fill in your sudo password into the password field.
3. Go to `System Preferences > Security & Privacy > Privacy`. In the Accessibility tab, make sure your Alfred 3 app is on the list.

## Note
It seems Apple's bug that Applescript can't access the property of password field in SecurityAgent window on macOS 10.13 (High sierra). If you encounter a problem that password won't be automatically filled into the field. Please gently click on the window of Security Agent, then it will continue.  

For more info, please refer to [here](https://forums.developer.apple.com/thread/83905)



