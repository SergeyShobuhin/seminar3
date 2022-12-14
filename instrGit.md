# **Инструкция по работе с системой контроля версий git**

![фото](овальчик.png)

## Инициализация репозитория

Команда создает в локальной директории(папке) пустой репозиторий в виде директории .git, где и будет в дальнейшем храниться вся информация об истории коммитов, тегах — о ходе разработки проекта:

        git init

## Проверка состояния репозитория

проверить состояние изменения, добавления и удаления файлов используем:

        git status

## Добавление версионности

временное хранилище(индекс) бля внениения изменений для последующего внесения в общий коммит:

        git add .\имя файла 

## Фиксация изменений

для фиксации всех изменений(все индексированные файлы) используем:

        git commit -m "commit коментарий"  // (также см. другие флаги "-a", "-am" и другие)

## Проверка истории коммитов

для проверки информации об коммитах изменивших файл испольхуем:

        git log  // общая информация    
        или 
        git log --флаг  // см. флаги --oneline(кратко в строку), -- all(в подробностях), --oneline -- all(полный граф коммитов, отводя по одной строке на коммит) и др.

## Проверка изменения в проекте

Сравнивает и показывает изменения в файлах команда:

        git diff  // по умолчанию разница между индексом и последним коммитом, можно чередовать индексы для их сравнения, так же см. другие флаги

## Переключение между ветками, извлечение отдельных файлов из истории коммитов

чтобы переключаться между последними коммитами (если
упрощенно) веток используем команду: 

        git checkout  // см. подробно master


## Ветвление

Описание ветвлений

### Просмотр существующих веток

        git branch // отобразит список веток


### Создание новых веток

        git branch <name> // <name> - имя ветки

### Слияние веток

        git merge <name> 

### Разрешение конфликта

1. определяем в чем конфликт
2. решаем

### Удаление веток

для удаления ненужных веток используем:

        git branch -d <name> 

## Удаленные репозитории

удаленные репозитории нужны для...

