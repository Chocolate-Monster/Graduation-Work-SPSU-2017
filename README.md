## Constructive method for analyzing the exponential stability of a system of differential equations with distributed delay.

#### Introduction
Differential equations with distributed delay are used to describe real processes in mathematical modeling. The speed of the process depends on its state at a given time, as well as on the previous states on a continuous time interval.  An important problem in the theory of differential equations is the problem of stability analysis.

In works by I.V. Medvedeva and A.P. Zhabko (see [4, 5] for systems with concentrated and [6] for systems with distributed delay) the sufficient condition for checking stability is shown. In [4, 5] a group of constructive methods for stability analysis of linear
differential-difference systems with a concentrated delay are proposed. My graduate work is devoted to generalization of methods [4,5] to the case of systems with distributed delay. 

This repository contains MATLAB code to test and demonstrate the method using an example of an equation:

![equation 1](https://user-images.githubusercontent.com/82182857/121483375-c928a300-c9d6-11eb-998b-ec84a7f7a378.jpg)


#### Algorithm

1. Choose an equation
2. Divide the investigated parameter space
into regions of stability and instability using the D-partitioning method. 
3. At each point in the area the algorithm should end with the same result, depending on the type of that area:

    * If the point is unstable, mark it on the graph with a black dot.
    * If the point is stable, mark it on the graph with a red cross.
    * If the point is not found to be stable, but can be found at greater N (the algorithm parameter responsible for linear approximation of the functional), mark it with a black cross.


The result of the algorithm is shown in figures 2 and 3 for N = 5 and N = 20 respectively.
From the results the following conclusions can be drawn:
* The stability and instability regions are correctly identified.
* With increasing N more and more points become "definitely" stable


![img 1](https://user-images.githubusercontent.com/82182857/121442245-e425f380-c993-11eb-9adc-45cf5d008cbc.jpg)


![img 2](https://user-images.githubusercontent.com/82182857/121442283-facc4a80-c993-11eb-8c9d-c605ad7765a1.jpg)


#### References:

<a id="4">[4]</a> 
Медведева И. В. Конструктивные методы анализа экспоненциальной
устойчивости линейных систем запаздывающего типа: дис. ... канд. физ.-
мат. наук. СПб., 2014. 150 с.

<a id="5">[5]</a> 
Medvedeva I. V., Zhabko A. P. Synthesis of Razumikhin and
Lyapunov–Krasovskii approaches to stability analysis of time-delay
systems// Automatica. 2015. Vol. 51. P. 372–377.

<a id="6">[6]</a> 
Медведева И. В., Жабко А. П. Анализ устойчивости линейных систем с
распределённым запаздыванием // Теория управления и математическое
моделирование: Тезисы докладов Всероссийской конференции с международным участием, посвященной памяти проф. Н.В. Азбелева и проф.
Е.Л. Тонкова (Ижевск, Россия, 9–11 июня 2015 г.). Ижевск: Изд-во «Удмуртский университет». 2015. С. 95-–96.
