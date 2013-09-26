nexus4_customize
================

Инструкции по прошивке

1 - Для Ubuntu нужно ставить adb и fastboot
sudo add-apt-repository ppa:nilarimogard/webupd8;sudo apt-get update; sudo apt-get install android-tools-adb android-tools-fastboot
Для Windows они лежат в папке с recovery

2 - Качаем recovery 



fastboot flash recovery ./adb/recovery/recovery-clockwork-6.0.3.6-mako.img
