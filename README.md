# MacOS give-control
A small shell script requiering sudo for giving a macos application permission to control the computer eg. read &amp; write keyboard events

# Instalation
Download and move into `/usr/local/bin` and run it by `give_control` (you might need  to run `chmod +x give_control` on it) or just start it by `sh ./give_control`

# Other permissions
this script can be edited to give control over these features:

![image info](./images/security_privacy.png)

by changing this code in the script:
```
# ******************* config *********************
Enable_Setting='kTCCServiceAccessibility'
# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```
to one of the options from
_[this list](https://github.com/AtlasGondal/macos-pentesting-resources/blob/main/tccd/kTCCService.md)_
