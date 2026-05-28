# 📅 День 1: Развёртывание jump-01

## 🖥️ Параметры ВМ
- ID: 101
- Имя: jump
- ОС: Debian 13.5
- vCPU: 2 (1 Core - 2 Sockets), RAM: 2 ГБ, Disk: 20 ГБ (VirtIO)
- Сеть: vmbr0 (Static), IP: 192.168.1.250

## ⚙️ Установка
- Разметка: /boot (1GB) + LUKS2 (LVM ---> VolumeGroup (Lv-swap swap (1GB), LV-main / (18GB))), ext4
- Пользователь: cyberded (sudo)
- Пакеты: ssh

## 🔑 Доступ
- SSH: пароль (keys ---> Day 2)
- QEMU Agent: ✅ 

## ✅ Проверки
- [+] apt update проходит
- [+] ssh cyberded@<IP> работает
- [+] hostname -I возвращает IP
