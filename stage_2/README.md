## Этап 2

**На данном этапе мы выберем модель, проведем обучение и сравнение результатов разных моделей (например catboost и линейных моделей Ridge и Lasso)**

## Ход работы:

1. **Обоснование выбора моделей:**
  - В качестве оценки сверху выбрана модель градиентного бустинга (CatBoost), поскольку она позволит нам оценить максимальный понециал, который можно получить из собранных данных. Данная модель более сложная и тяжело интерпретируемая.
  - В качестве основной модели выбрана модель линейной регрессии с L1 и L2 регуляризацией. Выбор модели обусловлен ее простотой и высокой интерпретируемостью.  
  
2. **Обучение моделей:**
    1) Обучение модели [градиентного бустинга][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/stage_2/CatBoost_model_car_market.ipynb]
    2) Обучение модели [линейной регрессии][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/stage_2/Leaner_regression_model.ipynb]

3. **Интерпретация результатов**
  
  В результате обучени 4 моделей были получены очень хорошие результаты, на графике приведены значения метрики R2 (Коэффициент детерминации) который рассматривают как универсальную меру зависимости одной случайной величины от множества других, в нашем случае таргета от признаков.

![Image alt](https://github.com/SergeyKulakin/Car_market_analysis/blob/98b9ece0c2812856756a617c0e33b1db3cdb832a/stage_2/screen/capture_20211226223932890.png)

4. **Вывод по работе**  
  
В данной работе были достигнуты следующие результаты:
  
  - Выполнен сбор и анализ данных с сайтов (Avto.ru, Drom.ru, Avito) в Московском регионе
  
На данном этапе   данные были обработаны и приведены к единому виду, организован общий DataSet всех объявлений с трех сайтов, выполнен первичный анализ.
 
  - Проведен разведочный анализ данных
 
На данном этапе все признаки в итоговом DataSet проанализированы и выбраны наиболее подходящие для обучения моделей
 
  - Обучение моделей и оценка результатов

На данном этапе было выполнено обучение модели градиентного бустинга CatBoost и линейных моделей Ridge, LASSO.
Были визуализированы предсказанные разными моделями (на тестовой выборке) значения целевой переменной. Интерпретация метрик и графиков подтверждает, что достигнуты значительные результаты в задаче предсказания цены автомобилей. Причем линейные модели в целях улучшения качеста модели были разделены на две (по целевой переменной до 3 млн. рублей и более 3 млн. руб.) модель градиентного бустинга выступила в качестве "планки" максимумального результата к которому следовало стремиться при обучении линейных моделей (оценка сверху).

**Таким образом, поставленные цели достигнуты.**
