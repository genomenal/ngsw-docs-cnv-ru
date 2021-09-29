---
sidebar_position: 3
sidebar_label: Отчет по CNV для пациента
---

# Отчет по CNV для пациента

Находится на вкладке **“Отчет по CNV”** на странице пациента.

![CNV report tab](/img/rus/34-cnv-report-tab.png)

Раздел **“Результат”** включает сообщение о наличии или отсутствии отклонения от нормального числа копий в какой-либо хромосоме во всех образцах пациента.

Раздел **“Интерпретация результатов и выводы”** содержит таблицу со следующей информацией по образцам пациента:

1. Обнаруженные отклонения (уменьшение или увеличение числа копий какой-либо хромосомы)
2. Покрытие образца
3. Особые отметки - сообщение о качестве данных:
- Нет отметки, если качество данных хорошее;
- “Имеются некритичные замечания к качеству данных”, если покрытие < 0,01X и/или данные не удовлетворяют всем критериям качества после очистки;
- “Результаты исключены из-за недостоверности. Слишком низкое покрытие секвенирования.”, если покрытие < 0,001X;
- “Анализ не проведен, программная ошибка”, если анализ образца завершился с ошибкой, упав на одной из стадий пайплайна.