## Регулятор оборотов ДПТ на таймере NE 555

### Состав репозиторая:

- печатные платы в формате *SpritLayout 6.0*
	- pwm_regulator.lay6
	- pwm_with_dc-dc.lay6
	- pwm_atx.lay6

	
> NB: Не забыть допаять защитный диод на двигатель там, 
> где он не предусмотрен на печатной плате
	
	
- в папке **ss555** - программа для расчёта номиналов элементов таймера для различных режимов работы.
- datasheet на сам таймер
- схемы устройства - schematics1.gif & schematics2.jpg
- книга Хоровица, Хилла **"Искусство схемотехники"**
- файл readme.md

### Компоненты:

- Таймер NE 555 в корпусе DIP
- Кроватка DIP8 под таймер
- Диоды D1, D2 - 1N4007
- Потенциометр B50k
- Транзистор IRFZ44N в корпусе TO-220
- Клеммные колодки 5 мм - 2 шт.
- Электролитический конденсатор (входной фильтр) 470 мкФ, 25 В
- SMD Резисторы и конденсаторы типоразмера 1206. Номиналы как на схеме


		R1 = 100
		R3, R4 = 1k
		C1 = 2,2 nF + 330 pF + 330 pF = 2,86 nF
		C2 = 1 nF
	
- Защитный диод - в зависимости от потребляемого нагрузкой тока. Выбран 1N4007

    (см. Хоровиц, Хилл стр. 59, о диодной защите ключа от индуктивной нагрузки)


### Ссылки

- http://electrik.info/main/praktika/685-shim-regulyatory-oborotov-dvigateley-na-taymere-555.html
- http://easyelectronics.ru/shim-regulyator-na-tajmere-ne555.html
