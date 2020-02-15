---
layout: page
title: About
permalink: /about/
---
# ![Awesome](http://www.amm.vsu.ru/images/logo.gif?raw=true) AMM

### Полезности:

Для подсчета времени выполнения можно посчитать разницу во времени до начала выполнения блока кода и после
~~~cpp
	clock_t start;
	clock_t stop;
	start = clock();
	for (int i = 0; i < 1000; ++i)
    {
        cout << "Random number : " << rand() % n;
	}
	stop = clock();
	double time = double(stop - start) / CLOCKS_PER_SEC;
	cout<<"time :"<<time<<endl;
    cin.get();
~~~
