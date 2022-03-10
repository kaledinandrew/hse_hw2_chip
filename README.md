# hse_hw2_chip

[Ссылка на колаб](https://colab.research.google.com/drive/1uDSwgJyl4dXfgFS-pTdyuSnm62u72dlU?usp=sharing)

Для исследования я выбрал клеточную линию **А549** с гистоновой меткой **H3K4me2**

## Статистика по выравниванию

|index|Общее количество ридов|Не выровнилось|Выровнилось уникально|Выровнилось больше 1 раза|
|---|---|---|---|---|
|ENCFF671XBU|44155295|38351885 \(86.86%)|1563249 \(3.54%)|4240161 \(9.60%)|
|ENCFF696CIT|35895288|31132107 \(86.73%)|1277589 \(3.56%)|3485592 \(9.71%)|
|ENCFF126TIE|22021226|18530461 \(84.15%)|785894 \(3.57%)|2704871 \(12.28%)|

## FastQC

### Реплика 1 (ENCFF671XBU)

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.00.06.png)

Все показатели в зеленой зоне (с небольшим уменьшением к концу), это говорит о хорошем качестве прочтений

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.00.56.png)
![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.01.30.png)

GC content очень похож на эталонный

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.01.50.png)

По этому графику понятно, что лишних адаптеров нет

Из этих графиков можно сделать вывод, что качество оказалось хорошим

### Реплика 2 (ENCFF696CIT)

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.02.41.png)

Качество хорошее, очень похоже на образец первой реплики

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.10.06.png)

GC content также очень близок к эталонному

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.03.31.png)
![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.04.02.png)

### Контроль (ENCFF126TIE)

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.04.22.png)

Качество прочтений похоже на оба предыдущих, хорошее

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.05.16.png)

GC content опять похож на эталонный

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.04.40.png)
![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.05.28.png)

Лишние адаптеры также не наблюдаются 

## Диаграмы Венна

Данные для пересечения X с Y не совпадают с пересечением Y с X, т.к. пересечение в данном случае считается как количество участков встречи в первом файле, которые встречаются и во втором тоже.

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.06.09.png)
![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.06.20.png)

Отсутсвие пересечений связано с тем, что мы производим выравнивание только на одну хромосому. Если бы выравнивание делали на все хромосомы, то шанс пересечения был бы больше.

![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.06.31.png)
![](https://raw.githubusercontent.com/kaledinandrew/hse_hw2_chip/main/images/Screenshot%202022-03-09%20at%2000.06.42.png)

## Бонусное задание

Бонусное задание см в [коллабе](https://colab.research.google.com/drive/1uDSwgJyl4dXfgFS-pTdyuSnm62u72dlU?usp=sharing)
