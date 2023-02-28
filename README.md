# Проект тестового задания на детекцию кораблей по спутниковым снимкам. 
Данная версия обучена на 1000 снимках с кол-вом эпох около 70, на завершение 100 эпох не хватило времени. Датасет был загружен с txt файлами разметки. В данной версии хотелось добиться точности распознования объектов.

В загруженом проекте присутствует файл с лучшими весами + снимки для тестов, без исходного датасета.

## Для проверки обученной модели следует выполнить следующие шаги:
1.Клонировать данный проект командой git clone https://github.com/Max10001/ShipDetector__WhenUsingDataset__

2.Перейти в папку виртульного окружения командой cd C:\Projects\ShipDetector(WhenUsingDataset)\venv\Scripts

3.Активировать виртуальное окружение командой activate

4.Вернуться в корневую папку проекта командой cd C:\Projects\ShipDetector(WhenUsingDataset)

5.Установить фреймворк yolo5 командой git clone https://github.com/ultralytics/yolov5

6.Перейти в папку фреймворка командой cd C:\Projects\ShipDetector(WhenUsingDataset)\yolov5

7.Установить библиотеки и зависимости проекта комнадой pip install requirements.txt

8.Для тестирования снимков, находящихся в папке images/test, использовать команду python detect.py --source C:\Projects\ShipDetector\images\test\ --weights runs/train/ship_det/weights/best.pt --conf 0.5 --name ship_det