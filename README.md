nexus4_customize
================

Инструкции по прошивке
// Если загрузчик разблокирован уже

1 - Для Ubuntu нужно ставить adb и fastboot
sudo add-apt-repository ppa:nilarimogard/webupd8;sudo apt-get update; sudo apt-get install android-tools-adb android-tools-fastboot
Для Windows они лежат в папке с recovery

2 - Скачиваем и распаковываем на компе архив: http://4pda.ru/forum/dl/post/3483937/Recovery.rar  ( 35.96 МБ )
  Скачиваем прошивку и загружаем в телефон в корень /sdcard


3 - Выключаем телефон и переводим его в Fastboot mode (зажимаем кнопки Volume Down + Power), подключаем USB-кабель. Драйвера должны быть установлены.
    
    if (Ubuntu)
      cd "в распаковонную папку"
      fastboot flash recovery ./adb/recovery/recovery-clockwork-6.0.3.6-mako.img # выбрать нужный образ
    еlseif (Windows):
      Для установки ClockworkMod Recovery 6.0.3.6
      запустить CWM 6.0.3.6.bat
      Для установки ClockworkMod Touch Recovery 6.0.3.6
      запустить CWM touch 6.0.3.6.bat
      Для установки Team Win Recovery Project 2.6.3.0
      запустить TWRP 2.6.3.0.bat
      Для установки Stock Recovery Android 4.2.2
      запустить Stock JDQ39.bat
      Для установки Stock Recovery Android 4.3
      запустить Stock JWR66Y.bat
    
    Готово
    
4 - Для входа в Recovery, в Fastboot mode клавишами громкости выбираем Recovery mode и подтверждаем выбор кнопкой питания.

5 - Делаем Backup

6 - Делаем
      wipe data/factory reset
      Wipe cache partition
      wipe dalvik cache
     
7 - Делаем 
 "install zip from sdcard" - "choose zip from sdcard"
 Выберите файлы (п.2 прошивку и Gapps) 
 и произведите их установку
 
 8 - Рекомендуется повторить "wipe data/factory reset"
 
 9 - Перезапускаем смарфтон - "reboot system" 
