# Потребление энергии СПбГЭТУ "ЛЭТИ"


Создание визуализации открытых энергетических данных о потребления энергии
СПбГЭТУ "ЛЭТИ".

## Предварительный просмотр

![](https://github.com/----------------------/preview.jpeg)

## Содержание
После того, как советники ректора университета обратились с призывом
экономить электроэнергию из-за угрозы переплаты электроэнергии осенью 2022 года,
был разработан данный сайт, для мониторинга электроэнергии по корпусам ЛЭТИ. К сожалению 
из за отсутствия новейших электросчетчиков которые могли бы передавать данные по сети, сайт 
разработан на примерной графике по потреблению главного счетчика СПбГЭТУ "ЛЭТИ". После разработки данного сайта
добавления новых счетчиков для новых пользователей не должно составить труда, поскольку коды дублируются.
Также нет необходимости закрыт доступ этих данных поскольку разработанный сайт полностью закрыт от внешнего доступа. 

## База данных
Общий объем электроэнергии, полученной из сети с главного электросчетчика в течение
15-минутные интервалы с 2022 года.

## Источники

### Линейный график

Линейный график основан на [этот код](https://github.com/arnauddri/d3-stock).
Были внесены следующие основные изменения:
- обновлено с d3 v3 до d3 v7
- разрешено изменение частоты данных (ежедневно, ежемесячно, ежегодно)
- удалена диаграмма областей посередине
- возможность отображать доверительные интервалы модели
- возможность отображения скользящей средней
- возможность показывать и скрывать разные линии
- возможность выбора между динамической и статической осью Y

### Тепловая карта календаря

Тепловая карта календаря основана на [этом коде](https://gist.github.com/alansmithy/6fd2625d3ba2b6c9ad48).
Были внесены следующие основные изменения:
- обновлено с d3 v3 до d3 v7
- возможность выбора отображаемых лет
- возможность выбора количества категорий

### Гистограмма

Гистограмма основана на [этот код](https://marcwie.github.io/blog/Response-bar-chart-d3/).
Были внесены следующие основные изменения:
- обновлено с d3 v4 на d3 v7
- разрешены отрицательные значения
- разрешено изменение частоты
- возможность выбора между абсолютными и относительными различиями

## About
Этот проект создан в рамках практики в СПбГЭТУ "ЛЭТИ"