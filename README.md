# act-common

Содержит схемные компоненты, схемы, общий код, инструменты, документы и т.д., применимые в области разработки проектов на базе микроконтроллеров, ПЛИС и т.д.

## Документы

Почти все документы, не относящиеся к "библиотечным элементам" (схемные символы, код), располагаются в общей WIKI по адресу https://dqxl1t0aqaave4.gitbooks.io/wiki/content/. Остальные располагаются под директорией '/doc'.

## Структура репозитория

В том числе и по историческим причинам во всех проектах, связанных с разработкой управляющих устройств, принята следующая структура каталогов:

1. `/doc` -- содержит текстовые и графические документы по задаче, которые нельзя положить в WIKI. В их числе отчеты, вспомогательные текстовые документы в бинарном формате, изображения. Файлы этой директории управляются `Git LFS`.
2. `/layout` -- содержит элементы разводки печатной платы (созданные, например, в `Sprint Layout 5.0`).
3. `/schema` -- содержит полноценные схемы-модели с возможностью тестирования, получения АЧХ и т.д., принципиальные схемы, схемные компоненты (созданные, например, `Micro Cap 9`)
4. `/mc` -- содержит исходный код проектов под микроконтроллер (например, проекты под `ATmega8A` в среде `IAR Embedded Workbench`).
5. `/pld` -- содержит схемы для ПЛИС (например, созданные в `Xilinx ISE`)
6. `/tool` -- содержит проекты-утилиты для ПК, обеспечивающие визуализацию отладочного вывода и управление поведением микроконтроллера (например, на `C++` под `Windows XP SP3` и выше в `Visual Studio 2013`).
7. `/lib` -- содержит внешние зависимости, например другие git-репозитории, включенные как submodule или subtree, зависимости, не имеющие собственных репозиториев, и т.д.

В данном репозитории вовсе не обязательно будут содержаться все каталоги. Однако при разработке аналогичных проектов следует придерживаться именно такой структуры.

За подробностями следует обращаться к `README.MD` соответствующих директорий.
