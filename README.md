# LR6
Лабораторная работа №6

**Студент:** Шевелёва Эвелина Сергеевна

**Группа:** 4317

# Отчет по работе с Git

## 1. Создание форка
Сделана копия в личное хранилище из https://github.com/Kurtyanik/LR6/

## 2. Установка Git
Установила Гит


## 3. Изменение имени пользователя
Команда для изменения имени пользователя:

```bash
$ git config --global user.name "4317 Шевелёва Э.С."
```
Команда для изменения почты пользователя:

```bash
$ git config --global user.email "shevelva.evelina@gmail.com"
```
*Результаты изменения имени и почты пользователя*

![Результаты изменения](./pictures/1.jpg)

## 4. Клонирование репозитория

```bash
$ git clone https://github.com/evasheveleva/LR6

```
*Скриншот с клонированием репозитория*

![Клонирование репозитория](./pictures/2.jpg)

## 5. Добавление нового файла

*Скриншот с добавлением нового файла*

![Добавление нового файла](./pictures/3.jpg)

## 6. Добавление изменений в локальный репозиторий

```bash
$ git pull
```


## 7. Получение данных для каждой из веток

```bash
$ git log --all --oneline
```

*Результат работы команды*

![Данные из веток](./pictures/4.jpg)

## 8. Просмотр последних изменений

```bash
$ git log -1
```

![Изменения](./pictures/5.jpg)

## 9. Решение конфликта и слияние веток

```bash
$ git checkout master
$ git merge origin/branch1
```
Решение конфликта с помощью текстового редактора путем замены содержимого mergefile.txt в ветке branch1
![Решение](./pictures/6.jpg)


## 10. Удаление побочной ветки после слияния

```bash
$ git push origin --delete branch1
```
*Результат работы команды*

![Удаление побочной ветки](./pictures/7.jpg)



## 11. Создание изменений и их фиксирование.

Создание нескольких изменений и коммиты для них

Для наглядной работы с репозиторием необходимо сделать изменения и зафиксировать их, оставляя комментарии. Поочередно в репозиторий были добавлены 4 текстовых файла: friends.txt, musicals.txt, town.txt, 1.txt.

![Создание файлов](./pictures/8.jpg)

## 12. Откат коммита

Откат к предыдущему коммиту:

```bash
$ git reset --hard HEAD~1
```
*Результат работы команды*

![Откат к предыдущему коммиту](./pictures/12.jpg)

## 13. Создание ветки для отчета
```bash
$ git checkout -b report
```
*Результат работы команды*

![Создание ветки](./pictures/10.jpg)

## 14. Получение истории операций в форматированном виде

```bash
$ git log --pretty=format:"%h %ad %an %s" --date=short
```

## 15. Логи команд

```bash
$ git config --global user.name "4317 Шевелёва Э.С."      (изменение имени)
$ git config --global user.email "shevelva.evelina@gmail.com"    (изменение почты)
$ git clone https://github.com/evasheveleva/LR6     (клонирование репозитория)
$ git pull   (добавление изменений)
$ git log --all --oneline    (получение данных)
$ git log -1    (просмотр изменений)
$ git checkout master
$ git marge origin/branch1   (слияние веток)
$ git push origin --delete branch1   (удаление ветки)
$ echo "бж пыль" >> friends.txt   (создание текстового файла)
$ git add friends.txt
$ git commit -m "1 файл"
$ echo "Twisted: The Untold Story of a Royal Vizier" >> musicals.txt
$ git add musicals.txt
$ git commit -m "2 файл"
$ echo "Коряжма" >> town.txt
$ git add town.txt
$ git commit -m "3 файл"
$ echo "+" >> 1.txt
$ git add 1.txt
$ git commit -m "4 файл"
$ git push
$ git reset --hard HEAD~1   (откат коммита)
$ git checkout -b report   (создание ветки для отчёта)
$ git log --pretty=format:"%h %ad %an %s" --date=short   (история операций)
```

## 16. История операций
Список истории операций:

+ 80ba56d 2024-11-22 4317 Шевелёва Э.С. Добавление рисунков
+ 36ddd8c 2024-11-22 evasheveleva Создание отчёта
+ d896340 2024-11-21 4317 Шевелёва Э.С. 3 файл
+ 086f2c2 2024-11-21 4317 Шевелёва Э.С. 2 файл
+ 4d649be 2024-11-21 4317 Шевелёва Э.С. 1 файл
+ be83e57 2024-11-21 4317 Шевелёва Э.С. Merge remote-tracking branch 'origin/branch1'
+ 5b0f07c 2024-11-21 evasheveleva Create main.cpp
+ 921f53b 2020-11-21 Kurtyanik Обновление информации
+ 0f9f50d 2020-11-21 Kurtyanik Заполнил файл
+ c08a654 2020-11-21 Kurtyanik Файл создан пустым
+ 3c6e913 2020-11-21 Kurtyanik Initial commit

