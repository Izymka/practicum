# Исследование закономерностей успешности игр

## Цель проекта
Анализ данных интернет-магазина "Стримчик" для выявления факторов успешности компьютерных игр. Результаты помогут:
- Определить перспективные платформы и жанры для продвижения.
- Спланировать рекламные кампании.
- Проверить гипотезы о влиянии рейтингов на продажи.

## Данные
Использованы исторические данные из открытых источников:
- Продажи игр по регионам (Северная Америка, Европа, Япония и др.).
- Оценки пользователей и критиков.
- Жанры и платформы (Xbox, PlayStation, PC и т.д.).

---

## Основные этапы анализа

### Предобработка данных
- **Проблемы в данных**:
  - Пропуски, аномалии и выбросы.
  - Несоответствие типов данных.
  - Нестандартные названия столбцов.
  
- **Решение**:
  - Удалены строки без названий игр (<0.1% данных).
  - Восстановлены пропуски:
    - Пользовательские рейтинги частично заполнены на основе оценок критиков.
    - Остальные пропуски заменены средними значениями по жанрам.
  - Для столбца `Рейтинг` добавлена категория **"Без рейтинга"**.

---

## Исследовательский анализ данных

### Динамика игровой индустрии
- Рост продаж начался после **1990 года**.
- **Топ-5 платформ по продажам**:
  1. PS2
  2. X360
  3. PS3
  4. Wii
  5. DS
- Средний срок популярности платформ: **6–10 лет** (кроме **PC** — вневременной спрос).

### Прогноз на 2017 год
- **Перспективные платформы**:
  - PS4
  - XOne
  - PC (стабильный спрос)
- **3DS** — пик популярности пройден.

### Влияние рейтингов
- Высокие оценки критиков (>8/10) коррелируют с продажами.
- Пользовательские рейтинги от **5/10** и выше обеспечивают стабильный спрос.

### Популярные жанры
| Регион        | Топ-3 жанра                | Антирейтинг                  |
|---------------|----------------------------|------------------------------|
| **Общий**     | Shooter, Platform, Sports  | Adventure, Puzzle, Strategy  |
| **Сев. Америка**| Action, Shooter, Sports  | -                            |
| **Европа**    | Action, Racing, Shooter    | -                            |
| **Япония**    | Fighting, RPG, Platform    | Shooter                      |

### Региональные предпочтения
- **Северная Америка и Европа**:
  - Платформы: X360, PS3, PS4.
  - Рейтинг: 10+.
- **Япония**:
  - Платформы: 3DS, PS3, PSP.
  - Жанры: Fighting вместо Shooter.

---

## Проверка гипотез
1. **Рейтинги Xbox One vs PC**:
   - Пользовательские оценки различаются (подтверждено статистически).
2. **Рейтинги Action vs Sports**:
   - Средние оценки для жанров **Action** и **Sports** не равны.

---

## Рекомендации для бизнеса
1. **Фокус на платформы**:
   - PS4, XOne (глобально).
   - 3DS (только для Японии).
   - PC (стабильный долгосрочный спрос).
2. **Продвижение жанров**:
   - Shooter, Sports, Platform (глобально).
   - Fighting и RPG (для Японии).
3. **Учет рейтингов**:
   - Приоритет играм с пользовательским рейтингом ≥5/10.
   - Экстремально высокие оценки критиков (>8/10) — маркер потенциального хита.
4. **Локализация стратегий**:
   - Для Европы акцент на Racing.
   - Для Японии — исключить Shooter из рекламных кампаний.

---

**Примечание**: Анализ выявил аномалии в данных. Рекомендуется регулярно обновлять выборку и проверять актуальность трендов.
