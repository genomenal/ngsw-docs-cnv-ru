---
sidebar_position: 2
sidebar_label: Пример образца с анеуплоидией и нормальным качеством данных
---

# Пример образца с анеуплоидией и нормальным качеством данных

Данными с нормальным качеством считаются те, у которых покрытие ≥ 0,01X и которые соответствуют всем критериям качества после очистки. Для образца с нормальным качеством данных все стадии пайплайна будут отмечены как завершенные и будет построен “Отчет по CNV”.

![41](/img/rus/41-main-page-normal-data-quality.png)
<p align="center">
<img src={require('/img/rus/41-main-page-normal-data-quality.png').default} width="800"/>
</p>

О наличии или отсутствии анеуплоидии можно узнать на вкладке “Отчет по CNV” на странице образца. Так, в данном образе наблюдается увеличение числа копий хромосомы 21.

<p align="center">
<img src={require('/img/rus/42-cnv-report-normal-data-quality-chr21.png').default} width="800"/>
</p>

Ту же информацию можно получить и на вкладке “Отчет по CNV” на странице пациента. Здесь же можно увидеть вердикт по качеству данных образца в колонке “Особые отметки”. В данном случае колонка пустая, что говорит о нормальном качестве образца.

<p align="center">
<img src={require('/img/rus/43-patient-cnv-report-normal-data-quality-chr21.png').default} width="900"/>
</p>