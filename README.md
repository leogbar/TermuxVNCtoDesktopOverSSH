# TermuxVNCtoDesktopOverSSH
Termux VNC Host to Desktop Client Over SSH

To install on Termux:

1. pkg install x11-repo #from https://hindux.github.io/setup-gui-in-termux/ now offline
2. pkg install tigervnc
3. pkg install xfce4
4. pkg install net-tools

5. vncserver -kill :1
6. vncserver :1
7. export DISPLAY=:1
8. startxfce4
9. whoami #give USER
10. passwd #put secure password and confirm
11. ifconfig #to get the IP_FROM_PHONE (see in wlan0)

Connect in Phone

1. On phone, install VNC Client, for example from F-Droid (MultiVNC) localhost:5901 (590X, X in DISPLAY)

![Image of Linux Ubuntu Login](https://raw.githubusercontent.com/leogbar/TermuxVNCtoDesktopOverSSH/master/Phone01.jpg) ![Image of Linux Ubuntu Login](https://raw.githubusercontent.com/leogbar/TermuxVNCtoDesktopOverSSH/master/Phone01.jpg)

Linux

1. On Linux, ssh -p 8022 -L 5901:localhost:5901 USER@IP_FROM_PHONE #SSH Server port in termux is 8022
2. On Linux, on VNC CLient use: localhost:5901

![Image of Linux Ubuntu Login](https://raw.githubusercontent.com/leogbar/TermuxVNCtoDesktopOverSSH/master/termuxVNCSSH.png)
