---
layout: post
title:  "Пример API для реализации sax парсера"
date:   2019-04-23 19:24:01 +0300
categories: results
---
# Пример API для реализации sax парсера

~~~cpp
#include <string>

using namespace std;

// Отдельные файлы .h .cpp
struct XmlHandler {
    
    void startDoc(void) {
        printf("startDoc");
    }
    
    void startTag(string tag) {
        printf("startTag");
    }
    
    void characters(string txt) {
        printf("characters");
    }
    
    void endTag(string tag) {
        printf("endTag");
    }
    
    void endDoc(void) {
        printf("endDoc");
    }
};

// Отдельные файлы .h .cpp
struct Parser {
    
    // Структура Parser содержит ссылку на handler
    XmlHandler* handler;
    
    // Возможность задать handler прямо при создании структуры
    Parser(XmlHandler* handler) {
        this->handler = handler;
    }
    
    void parseFile(string fileName) {
        // Пример вызова методов handler
        this->handler->startDoc();
    }
};

// Отдельный файл main.cpp
int main() {
    XmlHandler h = XmlHandler();
    Parser p = Parser(&h);
    p.parseFile("s");
}
~~~
