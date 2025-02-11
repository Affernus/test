# Исследование спроса на авиабилеты во время музыкальных фестивалей

**Задача:**  Необходимо проанализировать предпочтения пассажиров: на каких самолетах и в какие города летают больше. Кроме того, нужно выяснить, отличается ли  спрос на авиабилеты в города во время проведения в них музыкальных  фестивалей от спроса в другое время.

**Данные:** 3 csv-файла, от 8 до 101 объекта, от двух до четырёх признаков

**Библиотеки:** `pandas, numpy,collections, matplotlib, seaborn, plotly`

Данные получил при помощи SQL-запросов к базе данных Яндекс.Практикума.  Дополнил информацией о воздушных судах (пассажировместимость, дальность полёта, максимальная скорость), на основе новых признаков проанализировал число перевезённых пассажиров, сделал вывод о популярных рейсах и авиационных судах. Выполнил A/B тестирование в условиях ограниченного количества данных (10 объектов): сравнил средний спрос на авиабилеты в Москву во время музыкальных фестивалей и в остальное время. 

**Результат:** выяснил, что у пассажиров авиакомпании наиболее популярны ближне- и среднемагистральные рейсы (до 4500 км). Основные "рабочие лошадки" в авиапарке - это Сухой SuperJet-100. Больше всего летают в Москву (более 120 рейсов в день) и города в радиусе ближне- и среднемагистральной дальности от неё. 

Выявил неделю с аномально низкими продажами билетов, совпавшую с фестивальной. Несмотря на значимые отличия спроса в A/B тесте, заподозрил совпадение и рекомендовал провести дополнительное исследование с большим количеством данных, чтобы исключить влияние неучтённых факторов.