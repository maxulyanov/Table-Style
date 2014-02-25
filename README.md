Table-Style
===========

Плагин для оформления таблиц

##Описание

- Простой плагин на jQuery для оформления таблиц, имеющий встроенные шаблоны и множество пользовательских настроек.

##Установка

- Сбросить базовые стили или подключить блок RESET из файла style.css
- Подключить файл с темами theme.css
- Подключить последнию версию jQuery
- Подключить файл плагина jquery.tablestyles.js
- Вызвать плагин для нужной таблицы и передать в параметры пользовательские значения.

##Доступные параметры

###Глобальные параметры:
	- theme - выберет готовую тему
	- reset - параметр 'yes' отображает одну граница между ячейками таблицы
	- size - параметры 'small', 'middle', 'large' задает размеры ячеек

###Доступные темы:
	- GreyGreen-Simple
	- Green-Simple
	- DarkGrey-Simple
	
###Пользовательские параметры:
	- tableWidth - ширина таблицы, будет задана '50'
	- tableBorder - рамка таблица '1px solid red'
	- trBorderBottom - нижняя рамка для строки '1px solid red'
	- trBorderLeft - левая рамка для ячеек '1px solid red'
	- thBorderLeft - левая рамка для ячеек TH '1px solid red'
	- fontSize - размер шрифта для ячеек таблицы, будет задано в px '20'
	- fontSizeH - размер шрифта для ячеек заголовка TH, будет задано в px '20'
	- bgRow - Фон для ячеек '#f5f5f5'
	- bgRowH - Фон для ячеек заголовка TH '#f5f5f5'
	- bgRowEven - Фон для четных строк '#f5f5f5'
	- bgRowOdd - Фон для нечетных строк '#f5f5f5'
	- colorText - цвет текста таблица '#f5f5f5'
	- colorTextH - цвет текста заголовка TH '#f5f5f5'
	- colorTextEven - цвет текста для четных строк '#f5f5f5'
	- colorTextOdd - цвет текста для нечетных строк '#f5f5f5'
	- bgColFirst: - Фон для первой колонки таблицы '#f5f5f5'
	- colorColFirst - Цвет для первой колонки таблицы '#f5f5f5'
	- wColFirst - Ширина первой колонки таблицы, будет задан в px '100'
	- bgColLast -  Фон для последней колонки таблицы '#f5f5f5'
	- colorColLast - Цвет для последней колонки таблицы '#f5f5f5'
	
В конце каждого параметра показан пример пользовательского значения.
Все методы кроссбраузерны и избавляются от написания лишнего css, особенно при необходимости выбора чет/нечет. элементов, рамок(встроенный first-child) и т.д	
	
### Пример вызова плагина
$('#table').tablestyles({
	reset : 'yes',
	theme : 'GreyGreen-Simple',
	tableBorder : '5px solid #A5CE51',
});

Здесь для таблицы с ID table мы укажем значение параметра reset, установим тему GreyGreen-Simple и зададим значение для параметра tableBorder 
 
##Кроссбраузерность

 - IE8+ и все современные браузеры

##Пример работы

Можно посмотреть <a href="http://example.web-ulyanov.ru/frontend/table-style">Здесь</a>
