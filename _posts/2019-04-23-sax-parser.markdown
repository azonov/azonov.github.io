---
layout: post
title:  "1 курс 1 группа Результаты контрольной на функции"
date:   2019-04-20 19:24:01 +0300
categories: results
---
# Пример API для реализации sax парсера

~~~cpp
using namespace std;
#include <string>

struct XmlHandler {

void startDoc(void);

void startTag(string tag);

void characters(string txt);

void endTag(string tag);

void endDoc(void);
};

struct Parser {

Parser(XmlHandler* handler);

void parseFile(string fileName);
};

int main() {

}
~~~
