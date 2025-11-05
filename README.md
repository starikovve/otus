# otus
Administrator Linux. Professional

Обновление ядра системы


Цель домашнего задания
Научиться обновлять ядро в ОС Linux.
Описание домашнего задания
1) Запустить ВМ c Ubuntu.
2) Обновить ядро ОС на новейшую стабильную версию из mainline-репозитория.
3) Оформить отчет в README-файле в GitHub-репозитории.

Дополнительное задание:
Собрать ядро самостоятельно из исходных кодов.

проверим текущую версию ядра:
   uname -r
создвем и переходи в директорию kernel:
   mkdir kernel && cd kernel
качаем пакеты на виртуальную машину:   
   wget https://kernel.ubuntu.com/mainline/v6.18-rc4/amd64/linux-modules-6.18.0-061800rc4-generic_6.18.0-061800rc4.202511022101_amd64.deb
   wget https://kernel.ubuntu.com/mainline/v6.18-rc4/amd64/linux-image-unsigned-6.18.0-061800rc4-generic_6.18.0-061800rc4.202511022101_amd64.deb
   wget https://kernel.ubuntu.com/mainline/v6.18-rc4/amd64/linux-headers-6.18.0-061800rc4_6.18.0-061800rc4.202511022101_all.deb
   wget https://kernel.ubuntu.com/mainline/v6.18-rc4/amd64/linux-headers-6.18.0-061800rc4-generic_6.18.0-061800rc4.202511022101_amd64.deb
устанавливаем все пакеты сразу:
    sudo dpkg -i *.deb
перезагрузка
   reboot
просмотр истории команд и вывод их в файл README.md
   history
   history > README.md
