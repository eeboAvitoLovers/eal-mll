Проект кластеризации текстовых данных
Этот проект содержит реализацию модели кластеризации текстовых данных. Модель обучается на размеченных данных из файла raw_data.csv и сохраняется в файл model.pkl. Для визуализации результатов используется график распределения по кластерам distrib_by_class.png.

Установка зависимостей
Для установки необходимых зависимостей выполните следующую команду:


pip install -r requirements.txt
Обучение модели
Чтобы обучить модель, запустите скрипт fitting.py. Этот скрипт загружает обучающие данные из файла raw_data.csv, находит оптимальные параметры и сохраняет обученную модель в файл model.pkl.

Получение кластера новых данных
Чтобы получить кластер для новых данных, используйте скрипт visualization.py. Этот скрипт подключается к базе данных, считывает новые данные и вычисляет их кластер с помощью обученной модели. Затем он визуализирует распределение данных по кластерам с помощью графика distrib_by_class.png.

Формат данных
Файл raw_data.csv должен содержать два столбца: text и label. Столбец text содержит текстовые данные, а столбец label - их разметку.

Использование модели
Чтобы использовать обученную модель для кластеризации новых данных, загрузите ее из файла model.pkl и примените к новым данным.