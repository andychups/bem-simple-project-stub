# BEM Simple Project Stub
Супер-лайт Project Stub

# Концепции и технологии
* BEM – концепция блоков, состояний, уровней переопределений и т.п.;
* ENB – сборщик BEM-проектов;
* jQuery – уровень DOM;
* i-bem.js – BEM-фреймворк для построения Multi Page Application / Single Page Application;
* YModules – асинхронные модули;
* Backbone – модели и коллекции;
* Yate – клиент/серверый декларативный шаблонизатор;
* Stylus – препроцессор CSS.

# Шаблонизация (клиент/сервер): Yate + BEM + ENB
* Собирает все зависимости в бандлы;
* Собирает отдельно клиентские шаблоны;
* Вычитает дублирующие зависимости в common-бандл;
* Импортит common-бандл в page-бандл;
* Шаблоны находятся в одном "контексте" (page бандл с импортом common) и реиспользуют друг друга;
* Актуально для клиента: шаблоны могут вызываться точечно для перерисовки атомарных частей (блоков);
* Шаблоны на сервере и клиенте одинаковые.