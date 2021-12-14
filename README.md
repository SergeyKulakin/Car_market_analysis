# Car_market_analysis
This is repository about used car market analysis
# Анализ рынка б/у автомобилей

## **Команда:**
- Кулакин Сергей
- Исаакян Феликс
- Королёв Максим

## **Цель:**

- выяснить, как сильно разные характеристики влияют на цену б/у автомобилей;
- предсказать на реальных данных завышена или занижена цена на б/у автомобиль.

## **Задачи:**
1. cпарсить объявления на сайтaх:


- [Avto.ru][https://auto.ru/moskva/cars/all/?utm_source=google_adwords&utm_medium=cpc&utm_campaign=1536099723_place-gsearch_geo-msk-r1_type-brandovye-avtoru&utm_content=grid-67086384868_cat-brandovye-tochnyi-brand_land-all-list_view_geo-msk-r1&utm_term=автору_kwd-294813956142&gclid=Cj0KCQiAnaeNBhCUARIsABEee8VzZalGO1hwbSN4e-95T0Q5o8nyqdRYqq-eb9Fn2H-4yCAGt9XvEMcaAoT_EALw_wcB], 
- [Drom.ru][https://www.drom.ru], 
- [Avito][https://www.avito.ru/rossiya/avtomobili]; 


2. выбрать рынок б/у автомобилей в Москве или Санкт-Петербурга(что-то одно). Спарсить минимум 5000 объявлений;
3. обработать данные (выбросы, пропущенные значения);
4. провести разведочный анализ данных, попытаться понять какие характеристики (переменные) влияют на цены автомобилей. Для этого считать/визуализировать различные статистики в разрезе характеристик;
5. построить несколько линейных моделей и выбрать лучшую.

## **Ход работы:**
1. Код [парсинга Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Parser%20Avtoru.ipynb]
2. Код [парсинга Drom.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/collect_data_from_drom_ru.ipynb]
3. Код [обработки данных с Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Prepare_AvtoRu_Data_for_Analise.ipynb]
4. Код [обработки данных с Drom.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/drom_postprocessing.ipynb]
- Обработанные данные [с Avto.ru (Москва, 15289 объявлений, дата сбора данных - 27.11.2021)][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Data_avtoru_prep.xlsx]
- Обработанные данные [c Drom.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/drom_data_cleared.csv]
- Данные [с Avito (Москва, Mersers-Benz 5545 объявлений, дата сбора данных - 02.12.2021)][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Prep_data_from_avito.xlsx]
5. Код [Анализ признаков Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Analysis.ipynb]
6. Датасет []

## **Признаки в итоговом датасете**
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
