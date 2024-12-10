# Задание 3

## Переходим в нужную директорию и запускаем
Выполняем команды в терминале:

```
cd mongo-sharding-repl

docker-compose up -d  
```

## Инициализация шардирования и репликации
Для этого необходимо:
1. Подключиться к серверу конфигурации и провести инициализацию
2. Инициализировать реплицированные шарды
3. Инициализировать роутер и наполнить его данными

Все это упаковано в скрипт mongo-repl-init.sh

Запускаем скрипт в терминале:
```
./scripts/mongo-repl-init.sh
```

## Проверка результатов

Скрипт mongo-repl-check.sh покажет общее количество файлов, 
а так же количество файлов в репликах шардов и количество шард.

Запускаем скрипт в терминале:
```
./scripts/mongo-repl-check.sh 
```