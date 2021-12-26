## 1 Этап

## **Ход работы:**
1. Код [парсинга Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/stage_1/Parser%20Avtoru.ipynb]
2. Код [парсинга Drom.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/collect_data_from_drom_ru.ipynb]
3. Код [обработки данных с Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Prepare_AvtoRu_Data_for_Analise.ipynb]
4. Код [обработки данных с Drom.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/drom_postprocessing.ipynb]
- Обработанные данные [с Avto.ru (Москва, 15289 объявлений, дата сбора данных - 27.11.2021)][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Data_avtoru_prep.xlsx]
- Обработанные данные [c Drom.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/drom_data_cleared.csv]
- Данные [с Avito (Москва, Mersers-Benz 5545 объявлений, дата сбора данных - 02.12.2021)][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Prep_data_from_avito.xlsx]
5. Код [Анализ признаков Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Analysis.ipynb]
6. Датасет [https://github.com/SergeyKulakin/Car_market_analysis/blob/main/DATA.xlsx]

## **Признаки в датасете**
Датасет собран из двух путем объединения (Avtoru и Dromru)

- **name** - название с сайта
- **price** - цена авто (рубли) (int)
- **grade** - класс авто (от 1 до 10) (float)
- **year** - год выпуска авто (timestamp)
- **run** - пробег (км) (int)

- **back** - тип кузова
  - missed
  - внедорожник 5 дв. 
  - седан
  - хэтчбек 5 дв.
  - универсал 5 дв.
  - минивэн
  - лифтбек
  - купе
  - хэтчбек 3 дв.
  - компактвэн
  - пикап двойная кабина
  - пикап полуторная кабина
  - внедорожник 3 дв.
  - фургон 
  - купе-хардтоп
  - внедорожник открытый
  - седан 2 дв.
  - лимузин 
  - родстер 
  - кабриолет
  - фастбек

- **color** - цвет
  - черный
  - белый
  - серый
  - синий
  - серебристый
  - красный
  - коричневый
  - зеленый
  - бежевый
  - голубой
  - пурпурный
  - фиолетовый
  - желтый
  - оранжевый
  - золотистый
  - бордовый
  - розовый

- **tax** - налог (int)
- **transmission** - КПП
  - AT - автоматическая
  - MT - механическая
  - AMT - роботизированная
  - CVT - вариатор

- **drive** - привод
  - передний
  - полный
  - задний

- **rudder** - руль
  - левый
  - правый

- **owners** - количество владельцев (int)
- **pasport** - ПТС автомобиля
  - missed - нет информации
  - Оригинал
  - Дубликат

- **cr_date** - дата публикации объявления (timestamp)
- **views** - количество просмотров объявления (int)
- **comment** - комментарий продавца
- **engine_volume** - объем двигателя (литры) (float)
- **horsepower** - лошадиные силы (л.с.) (int)
- **engine_type** - тип двигателя
  - бензин
  - дизель
  - газ
  - электро
  - гибрид

- **car_brand** - марка авто
- **car_model** - модель авто
- **log_price** - логарифм цены (float)
- **car_age** - возраст автомобиля (дни) (int)
- **popularity** - популярность объявления (просмотры / дни публикации) (float)
