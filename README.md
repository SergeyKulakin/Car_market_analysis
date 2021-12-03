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
2. Код [обработки данных с Avto.ru][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/Prepare_AvtoRu_Data_for_Analise.ipynb]
- Обработанные данные [с Avto.ru (Москва, 15770 объявлений, дата сбора данных - 27.11.2021)][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/AvtoRu_prep.xlsx]
- Обработанные данные [с Avito (Москва, Mersers-Benz 5545 объявлений, дата сбора данных - 02.12.2021)][https://github.com/SergeyKulakin/Car_market_analysis/blob/main/AvtoRu_prep.xlsx]
