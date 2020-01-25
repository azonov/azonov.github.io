---
layout: page
title: About
permalink: /about/
---
# ![Awesome](http://www.amm.vsu.ru/images/logo.gif?raw=true) AMM

### Полезности:

Для подсчета времени выполнения можно посчитать разницу во времени до начала выполнения блока кода и после
https://www.icloud.com/keynote-live/sc:0z8kfY6Jq9I7loWTrqRH6TUjcJRuf6wjfFIUFE9U-B5a8s0AE44J9NAxIBbPcZGPrrR
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
