## Предсказание заказов такси

**Общее описание задачи.**<br>
Чтобы привлекать больше водителей в период пиковой нагрузки на исторические данных о заказах такси в аэропортах нужно спрогнозировать количество заказов такси на следующий час.  

**Данные.**
Входные данные представляют собой временной ряд заказов такси в десятиминутном таймфремею 

**Задача.**
Обучить несколько моделей предсказания заказов такси и выбрать лучшую модель по метрике RMSE. Значение метрики RMSE на тестовой выборке должно быть не больше 48.

# Используемые инструменты
**Библиотеки и модули**
pandas, numpy, os, matplotlib, statsmodels, sklearn

from statsmodels.tsa.seasonal import seasonal_decompose
from statsmodels.tsa.stattools import adfuller
from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
from statsmodels.iolib.table import SimpleTable

**Модели**
RandomForestRegressor, lightgbm, SARIMAX

**Метрики**
mean_squared_error
