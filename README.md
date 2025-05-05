# football_analytics

## 📌 Цель
Исследовать, как стиль игры (скорость атаки, тип передач, защитный прессинг) влияет на результативность команд на основе данных European Soccer Database.

## 🔍 Данные
- Источник: [European Soccer Database на Kaggle](https://www.kaggle.com/datasets/hugomathien/soccer) (файл `database.sqlite`, 100+ МБ).    
- Использованные таблицы:  
  - `Match` (голы, ID команд)  
  - `Team_Attributes` (параметры атаки и защиты).
  - `Player` (имена игроков, ID игроков)  
  - `Team` (название команд, ID команд)  
  - `League` (название лиги, ID лиги)    

## 📊 Методы
1. **Статистический анализ:**  
   - t-тест для сравнения скорости атаки.  
   - ANOVA для типа передач.  
2. **Визуализация:**  
   - Seaborn/Matplotlib (boxplot, scatterplot).  
3. **Инструменты:**  
   ```python
   sqlite3, pandas, scipy, sklearn, Matplotlib, jupyter

## 🚀 Ключевые результаты
Команды с короткими передачами забивают больше голов (p < 0.001):
Голы по типу передач

Скорость атаки не влияет на результативность (p = 0.299).

Топ-3 команды по defence pressure: Bayern, Juventus, Chelsea.

## 🛠 Запуск
Установите зависимости:

bash
pip install -r requirements.txt
Скачайте database.sqlite.

## Откройте Jupyter Notebook:

bash
jupyter notebook analysis.ipynb
