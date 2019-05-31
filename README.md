# Atomic Pi ClusterBlitz

## Logging into a Fresh Atomic Pi
* Connect Atomic Pi to keyboard, mouse, HDMI monitor and Ethernet LAN.
* Power on Atomic Pi and wait for device to boot.
* If the device tries to netboot over IPv4 and IPv6 simply press Esc.  It may cycle through this twice on its initial powerup.
* Login with default password supplied on the screen.
* Open Terminal (Ctrl + Alt + t)
* Change the password for the atomicpi account
  ```bash
  sudo passwd atomicpi
  ```
* Change the hostname for the atomicpi
  ```bash
  sudo hostnamectl set-hostname atomicX
  ```
* Restart the APi
  ```bash
  sudo restart
  ```
* Allow the APi to restart then login with your new password
* Verify that sshd is running
  ```bash
  sudo systemctl status sshd
  ```
* You can now unplug the keyboard, mouse, and hdmi and repeat this process for the rest of your APi's.  I set the password the same for all nodes and followed the hostname naming structure of atomic(1-3).

