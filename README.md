# TermuxVNCtoDesktopOverSSH
Termux VNC Host to Desktop Client Over SSH

Write on Termux terminal:

1. pkg install x11-repo #from https://hindux.github.io/setup-gui-in-termux/ now offline
2. pkg install tigervnc
3. pkg install xfce4
4. export DISPLAY=:1
5. startxfce4

Phone

6. On phone, install VNC Client, for example from F-Droid (MultiVNC) localhost:5901 (590X, X in Display)

Linux

7. On Linux, ssh -p 8022 -L 5901:localhost:5901 IP_FROM_PHONE #SSH Server IP is 8022
8. On Linux, on VNC CLient use: localhost:5901

