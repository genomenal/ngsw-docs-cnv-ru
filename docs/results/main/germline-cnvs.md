---
sidebar_position: 1
sidebar_label: Герминальные вариации числа копий
---

# Герминальные вариации числа копий

Обнаруженные и аннотированные участки числа копий можно скачать в формате AnnotSV CSV ![Table file](/img/rus/22-table-file.png) , 
в виде файла покрытия CNV в формате TSV ![CNV coverage file](/img/rus/23-cnv-coverage-file.png) , 
открыть в облаке Google в виде таблицы ![Google Cloud file](/img/rus/24-google-cloud-icon.png) .
Полногеномный график сегментов CNV можно открыть и скачать в формате PNG ![Plot file](/img/rus/25-plot_file.png) .
График по типу кариограммы с обозначенными CNV уровня хромосом можно открыть и скачать в формате PNG ![Karyotype file](/img/rus/26_karyotype_file.png) .
Также Вы можете открыть модуль визуализации вариаций на геноме 
во встроенном IGV ![IGV](/img/rus/27_igv.png) .

**AnnotSV CSV **- таблица аннотированных участков изменения копий. Они представлены как в виде полной делеции или инсерции, 
так и в виде разбитых на гены участков внутри делеции/инсерции.

**Основные поля описания варианта (AnnotSV CSV)**

<table>
  <tr>
   <td>Поле
   </td>
   <td>Описание
   </td>
  </tr>
  <tr>
   <td>AnnotSV ID
   </td>
   <td>ID варианта, присваемый аннотатором
   </td>
  </tr>
  <tr>
   <td>SV chrom
   </td>
   <td>Хромосома
   </td>
  </tr>
  <tr>
   <td>SV start
   </td>
   <td>Начало участка
   </td>
  </tr>
  <tr>
   <td>SV end
   </td>
   <td>Конец участка
   </td>
  </tr>
  <tr>
   <td>SV length
   </td>
   <td>Длина участка
   </td>
  </tr>
  <tr>
   <td>SV type
   </td>
   <td>Тип изменения числа копий (DEL, DUP)
   </td>
  </tr>
  <tr>
   <td>AnnotSV type
   </td>
   <td>Тип записи (full - участок целиком, split - участок, разбитый погеново). Каждому full-участку могут соответствовать несколько split-участков.
   </td>
  </tr>
</table>

Описание остальных 54 полей аннотации можно найти по ссылке: [AnnotSV Manual](https://lbgi.fr/AnnotSV/Documentation/README.AnnotSV_latest.pdf).


**Файл покрытия CNV** - неаннотированный файл в формате, удобном для рассмотрения изменения копийности на крупных участках (плечи хромосом, хромосомы).

**Основные поля описания варианта (файл покрытия CNV)**

<table>
  <tr>
   <td>Поле
   </td>
   <td>Описание
   </td>
  </tr>
  <tr>
   <td>ID
   </td>
   <td>Название участка (плеча, хромосомы)
   </td>
  </tr>
  <tr>
   <td>Call
   </td>
   <td>Вердикт по количеству копий. Принимает значения + (увеличенное количество копий по сравнению с нормой), - (уменьшенное число копий по сравнению с нормой), . (не было замечено отклонений в числе копий) и Not considered (локус вообще не рассматривался при анализе).
   </td>
  </tr>
  <tr>
   <td>Ampl_cov
   </td>
   <td>Покрытие (в нуклеотидах) эффективной длины локуса сегментами с количеством копий выше порога амплификации
   </td>
  </tr>
  <tr>
   <td>Ampl_cov_frac
   </td>
   <td>Доля (в %) эффективной длины локуса, покрытая сегментами с количеством копий выше порога амплификации
   </td>
  </tr>
  <tr>
   <td>Chrom
   </td>
   <td>Хромосома
   </td>
  </tr>
  <tr>
   <td>Depl_cov
   </td>
   <td>Покрытие (в нуклеотидах) эффективной длины локуса сегментами с количеством копий ниже порога деплеции
   </td>
  </tr>
  <tr>
   <td>Depl_cov_frac
   </td>
   <td>Доля (в %) эффективной длины локуса, покрытая сегментами с количеством копий ниже порога деплеции
   </td>
  </tr>
  <tr>
   <td>Effective_end
   </td>
   <td>Максимальное значение координаты эффективной длины
   </td>
  </tr>
  <tr>
   <td>Effective_length
   </td>
   <td>Суммарная эффективная длина
   </td>
  </tr>
  <tr>
   <td>Effective_start
   </td>
   <td>Минимальной значение координаты эффективной длины
   </td>
  </tr>
  <tr>
   <td>End
   </td>
   <td>Координата конца биологической сущности        
   </td>
  </tr>
  <tr>
   <td>Length
   </td>
   <td>Длина биологической сущности
   </td>
  </tr>
  <tr>
   <td>Start
   </td>
   <td>Координата начала биологической сущности
   </td>
  </tr>
</table>


**Полногеномный график сегментов CNV (пример)**

<p align="center">
<img src={require('/img/rus/28-genome-wide-plot.png').default} width="800"/>
</p>

На горизонтальной шкале мы видим хромосомы, по вертикали - копийность хромосомы. Так, для этого образца копийность хромосомы 21 увеличена в несколько раз.

**График по типу кариограммы с обозначенными CNV уровня хромосом (пример)**

<p align="center">
<img src={require('/img/rus/29-karyotype-plot-example.png').default} width="500"/>
</p>

На кариограмме обозначено, что в образце наблюдается увеличение числа копий хромосомы 21.
