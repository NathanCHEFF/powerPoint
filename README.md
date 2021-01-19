# powerPoint
Предлагаю вашему, внимаю предложение по доработке и совершенствованию схем питания переносных измерительных приборов.
Устройство предназначено для обеспечения питания для измерительных приборов, работающих на низковольтном постоянном напряжении,
широкого диапазона величин (от двух до 35 вольт). Устройство легко в сборке, имеет малые габариты и вес.
Устройством можно заменять внутреннее питание переносных измерительных приборов.

Устройство состоит из:

- Контроллер питания tp4056 требуется для качественной зарядки аккумуляторной батареи. Может автоматически изменять ток заряда батареи.
Основан на контроллере, который заряжает cv/cc методом(контроль напряжения/контроль тока), что увеличивает срок эксплуатации батареи.
- Батарея 18650. Элемент хранения Энергии, для последующей эксплуатации для питания потребителей.
- преобразователь напряжения повышающий, регулируемый HW441, позволяет преобразовать напряжение, накопленное в аккумуляторе. Регулируя его в широком диапазоне.

Эконом расчет:
Допустим Емкость батареи =~ 3200mA/час == 3.2А.
Допустим ток потребления нагрузки 50мА.

(Емкость батареи / ток потребления нагрузки) / 24 = (3.2 / 0.05) / 24 = 2.66 дней беспрерывной(!) работы.
Батарея типа «Крона» имеет ёмкость (по паспорту) 0,5 А·ч (щелочной "кроны" - 625 мА*h), Округлим это значение до 1000мА/h.
(1000 / 0.05) = 14 часов беспрерывной работы.

Сравнение по себестоимости с элементом питания типа крона:
- Стоимость HW441: 1$;
- tp4056: 0.3$
- батарея 18650: 1$

- По статистике сайта prom (https://prom.ua/Batarejka-krona-schelochnaya;2.html) цены на кроны варьируются от 1 до 4 $.

По моему субъективному мнению, исходя приведенных выше расчетов, целесообразно было бы перейти на автономное питание, так как
1 - по цене 2‑х хороших батарей, типа "крона" можно собрать устройство, которое в 3.2 раз превосходит по емкости этих двух крон.
Емкость аккумулятора /(паспортная емкость кроны * количество ).
Также прогнозирую экологический эффект, так как за жизненный цикл li-ion батарей в n циклов разряда, можно сменить
[ (время разряда аккумулятора (ч)/ время разряда кроны) * n = ] Батарей типа "крона".




