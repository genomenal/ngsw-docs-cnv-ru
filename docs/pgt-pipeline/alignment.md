---
sidebar_position: 4
sidebar_label: Выравнивание
---

# Выравнивание

Для поиска вариантов прочтения должны быть картированы на референсный геном. В Genomenal мы используем наиболее современную версию генома [GRCh38](https://www.ncbi.nlm.nih.gov/assembly/GCF_000001405.26/).
Процесс проходит в несколько этапов.

## 1. Проверка и восстановление парности прочтений

При использовании парного секвенирования (в этом случае фрагменты ДНК секвенируют с каждого конца навстречу друг другу) для картирования необходимо, чтобы каждое прочтение из одного файла содержало пару во втором. При фильтрации парность может быть нарушена, поэтому мы удаляем прочтения, которые лишились пары на предыдущих этапах.

## 2. Выравнивание

На этом этапе определяется местоположение прочтений на референсном геноме. Genomenal выполняет эту процедуру при помощи [BWA Burrows-Wheeler Aligner](http://bio-bwa.sourceforge.net/) (алгоритм MEM), рекомендуемого сообществом для этих целей инструмента.

## 3. Вычисление покрытия

Для оценки качества картирования на интересующих Вас областях (генах, транскриптах) мы рассчитываем понуклеотидное покрытие на геноме, а также среднее покрытие на целевой области (полный геном, экзом, панель). Результаты этого этапа можно увидеть на вкладке **“Анализ покрытия”.**
