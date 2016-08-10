# component-zmicron-Bootstrap_v3.3.4
ZMicron component

Переменные фреймворка можно настроить через файл i/css/dev/bootstrap3/variables.less. Подключение компонента:

IncludeCom("dev/bootstrap3");

Так же если вы используете бутстрап или его компоненты (не только в админке), то важно знать что в движке уже есть базовые css стили и css нормализатор, который конфликтует с аналогичными модулями в bootstrap3. Поэтому если у вас на сайте используется bootstrap3, то из файла tpl/main_tpl.php нужно удалить следущие строки:

<link rel="stylesheet" type="text/css" href="<?= Root('i/css/normalize.css')?>" />
<link rel="stylesheet" type="text/css" href="<?= Root('i/css/main.css')?>" />

Сами файлы /i/css/normalize.css и /i/css/main.css тоже можно удалить
