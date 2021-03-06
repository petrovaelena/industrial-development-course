# Слайды и конспекты лекций по дисциплинам «Промышленная разработка» и «Социально-управленческие аспекты промышленной разработки»

## Содержимое репозитория

* Каталог `technical` содержит слайды и конспекты по дисциплине «Промышленная разработка».
* Каталог `social` содержит слайды и конспекты по дисциплине «Социально-управленческие аспекты промышленной разработки».
* Каталог `example` содержит пример слайдов одной полноценной лекции. Приведён для справки.
* Файл `industrial-development.cls` является стилевым файлом для слайдов по обоим предметам. Не изменяйте его!

## Порядок работы

1. Войдите в каталог, соответствующий предмету, по которому собираетесь готовить слайды (см. выше).
2. Скопируйте файл шаблона `template.tex` тот же самый каталог, где он находится, под новым именем, образованным следующим образом: `<номер темы двумя цифрами>_<название темы по английски>.tex`. Например, `01-requirement-elicitation.tex`.
3. Откройте полученный на предыдущем шаге `.tex`-файл. Заполните аргументы команд `\title` и `\author`. Заполните аргумент команды `\graphicspath` таким образом, чтобы он совпадал с именем `.tex`-файла, но вместо расширения `.tex` заканчивался символом `/` (например, `\graphicspath{{01-requirement-elicitation/}}`) — это будет название подкаталога для хранения вспомогательных файлов (например, изображений).
4. Подготовьте контент слайдов и конспект лекции в соответствии с образцом в файле. Обратите внимание, что конспект лекции по умолчанию не попадает в итоговый pdf. Чтобы его увидеть, нужно исправить первую команду `.tex`-файла следующим образом: `\documentclass[lecturenotes]{../industrial-development}`.
5. Добавьте файлы изображений (желательно векторные) в каталог, описанный в п. 3. По возможности вместе с файлом изображения положите его исходник в редактируемом формате.
6. По окончании подготовки материалов уберите опцию `[lecturenotes]` из первой строки `.tex`-файла, если она там есть, добавьте `.tex`-файл и необходимые файлы изображений в систему контроля версий и зафиксируйте внесённые изменения. Обратите внимание, что скомпилированный `.pdf`-файл не должен попасть в репозиторий!
7. Отправьте внесённые изменения на сервер, избегая слияний и создания новых веток.
