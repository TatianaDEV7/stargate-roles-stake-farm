# stargate-roles-stake-farm
Оригинал: https://github.com/razeb-in-sec/stargate-roles-stake-farm

# Видео для запуска на Windows
https://www.youtube.com/watch?v=NByZEnvVmjQ

> ВАЖНО: в именах папок не должно быть пробелов!!!!

Делаем все по видео гайду.

#### Команды установки пакетов в видео
Для удобства вставлю здесь команды которые запускаются в видео.
- Это установка нужной версии библиотеки Web3:
```
pip install web3==5.31.1
```
- Это остальные пакеты:
```
pip install web3 requests datetime termcolor cprint time json random syspip install tqdm ccxt loguru termcolor telebot pyuseragents tabulate
```

# Команды для запуска на Ubuntu
Скачать репозиторий
```
git clone --branch=TatianaDEV7-branch-1 https://github.com/TatianaDEV7/stargate-roles-stake-farm
```
установим нужные пакеты
```
pip install python3-pip tqdm ccxt loguru termcolor telebot pyuseragents tabulate web3==5.31.1
```
Запускать процесс будем фоном с помощью tmux. Установим tmux:
```
sudo apt update && sudo apt install tmux -y
```
Запускаем сессию тмукс:
```
tmux new -s stargate-script
```
Переходим в папку со скриптом:
```
cd stargate-roles-stake-farm
```
Теперь запускаем сам скрипт:
```
python3 main.py
```

### tmux команды
Выходим из сессии `Ctrl+b d` (Но сессия ДАЛЬШЕ продолжит работать в фоне): 

Лист с сессиями
```
tmux ls
```
Опять конектимся к сессии
```
tmux attach -t stargate-script
```
> !Только не закрывайте скрипт с помощью CTRL+C 
