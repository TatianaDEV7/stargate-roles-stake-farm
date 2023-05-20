# stargate-roles-stake-farm
Оригинал: https://github.com/razeb-in-sec/stargate-roles-stake-farm
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
