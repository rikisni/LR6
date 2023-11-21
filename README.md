# LR6
Лабораторная работа №6
# Лабораторная работа №6
### Цель лабораторной работы
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием. 
### Ход работы
1) Создал аккаунт на GitHub ([рис. 1](https://github.com/rikisni/LR6/blob/master/image/1.png?raw=true)).
2)	Сделал копию (fork) в личное хранилище из [репозитория](https://github.com/Kurtyanik/LR6/) ([рис. 2](https://github.com/rikisni/LR6/blob/master/image/2.png?raw=true)).
3)	Установил Git.
4)	После установки настроил клиент git, введя имя пользователя (4216 Domanov) и email ([рис. 3](https://github.com/rikisni/LR6/blob/master/image/3.png?raw=true)).
```d
git config --global user.email "domanov.044@gmail.com"
git config --global user.name "4216 Domanov"

```
5)	Клонировал свой личный удалённый репозиторий на компьютер ([рис. 4](https://github.com/rikisni/LR6/blob/master/image/4.png?raw=true)).
```d
git clone https://github.com/rikisni/LR6
```
6)	Добавил файл `jfile` через интерфейс GitHub. Подтянул изменения в локальный репозиторий.
```d
git pull
```
7) Получил историю операций для всех веток ([рис. 5](https://github.com/rikisni/LR6/blob/master/image/5.png?raw=true)).
```d
git log --oneline --all
```
8)  Посмотрел последние изменения.
```d
git branch -v
```
9) Выполнил слияние в ветку `master`, разрешив конфликт ([рис. 6](https://github.com/rikisni/LR6/blob/master/image/6.png?raw=true).
```d
git merge 
```
10) Удалил побочную ветку после успешного слияния ([рис. 7](https://github.com/rikisni/LR6/blob/master/image/7.png?raw=true)).
```d
git branch -d branchtest
```
11) Сделал изменения и зафиксировал их, оставляя комментарии несколько раз ([рис. 8](https://github.com/rikisni/LR6/blob/master/image/8.png?raw=true)).
```d
git add .
git commit -m "comment"
```
12) Сделал откат коммита ([рис. 9](https://github.com/rikisni/LR6/blob/master/image/9.png?raw=true))
```d
git reset --soft HEAD~
```
13) Создал ветку для отчета ([рис. 10](https://github.com/rikisni/LR6/blob/master/image/10.png?raw=true)).
```d
git checkout -b отчетная_ветка
```
14) Оформил отчет в файле `README.md`
15) Получил историю операций в форматированном виде ([рис. 11](https://github.com/rikisni/LR6/blob/master/image/11.png?raw=true)).
```d
git log --pretty=format:'%h %cd | %an | %s' --date=format:'%F %R'
```
### Вывод
Изучил базовые возможности системы управления версиями, получил опыт работы с Git Api, опыт работы с локальным и удаленным репозиториями. 
