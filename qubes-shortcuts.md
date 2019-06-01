# Qubes OS shortcuts

## Standard shorcuts

You can find them in:
* Menu -> System Tools -> Keyboard -> Application Shorcuts
* Menu -> System Tools -> System Manager -> Window Manager -> Keyboard


Commonly used [Qubes OS](https://www.qubes-os.org/) shortcuts:

* `Alt+F3` : open application finder

* `Ctrl+Alt+Del` or `Ctrl+Alt+L` : lock the screen

* `Print` : print whole screen

* `Alt+Print` : print current window

* `Ctrl+Alt+Left/Right` : display the left/right workspace

* `Ctrl+Alt+Home/End` : move current window to left/right workspace

* `Ctrl+Alt+D` : Show desktop

Others:
* `Fn+Bightness +/-` : Change Brightness Up/Down


## Custom application shorcuts

To add a custom application shorcut:
* Click `Menu -> System Tools -> Keyboard -> Application Shorcuts`
* Click `Add`
* Enter the desired application `Command` and click OK
* Enter the desired shorcut with the keyboard

Application commands:
* `amixer set Master 5%+` : Volume Up
* `amixer set Master 5%-` : Volume Down
* `amixer set Master toggle` : Volume Mute/Unmute

## Application Finder shorcuts
Sometimes the quickest way to start an application is to use the Application Finder and enter the app phrase.
* `Alt+F3` + `vmName: applicationName` + `2x Enter`

Common app phrases:
* `vmName: ter` - starts the Terminal
* `vmName: fire` - starts Firefox

If you use often the application finder shortcuts, you might like to rename your VM to a few letters. For example from `personal` to `p`. Then you can start Firefox just with phrase `p: fire`.
