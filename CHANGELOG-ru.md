# CHANGELOG

## 1.2.2

- Отображение текущего количества юнитов каждого типа

## 1.2.1

- Исправлено мигание при использовании отладочного интерфейса внутри `get_action`
- Сущности в `player_view` теперь отсортированы по id

## 1.2.0

- Сохранение/загрузка состояния игры
- Исправлено случайное поведение при фиксированном сиде
- Контролирование выполнения команд отладочного интерфейса для избежания мигания
- Отладочное обновление теперь получает состояние игры которое отрисовывается (учитывается перемотка)
- Отладочные данные, переданные во время отладочного обновления, контролируют глобальное хранилище отладочных данных
- Добавлена библиотека `itertools` в Rust
- Улучшена производительность клиента Ruby

## 1.1.1

- Добавлена библиотека `pandas` в PyPy

## 1.1.0

- Рандомизированный порядок атаки

## 1.0.0

- Добавлены библиотеки `pandas` & `torch` в Python

## 0.4.1-beta

- Изменены очки за постройку и уничтожение турели

## 0.4.0-beta

- В матчах 1 на 1 (Финал), если остается один игрок, ему добавляются очки, достаточные для победы
- Юниты-строители теперь могут ремонтировать других юнитов
- Динамическая стоимость теперь применяется только для юнитов
- Уменьшена стоимость турелей
- Уменьшены очки за уничтожение стены
- Исправлен неработающий параметр `break_through` при отсутствии действия атаки
- Изменена версия Python на 3.8 и добавлена библиотека `numba`
- Добавлены `rand` & `chrono` в пакет языка Rust
- Добавлены примеры для быстрого старта на Python, C++, C# и Java

## 0.3.0-beta

- Новая механика движения
- Динамичная стоимость строительства
- Уменшена скорость ремонта
- Добавлен numpy в PyPy
- Изменен интерпретатор Ruby на JRuby

## 0.2.2-beta

- Улучшения в схематичной отрисовке
- Заканчивать игру если остался один (или ноль) игроков
- Добавлен PyPy

## 0.2.0-beta

- Усилена валидация значений на сервере
- В Раунде 2 и Финале в начале также дается база строителей
- Добавлены значения свойств сущностей в правила
- Изменения в свойствах сущностей
- Изменен порядок обработки действий - теперь, сперва действия атаки обрабатываются для всех сущностей, затем действия строительства, ремонта и движения аналогично
- Начальное положение камеры по центру мира
- Сохранение положения камеры
- Настройка `break_through` теперь не пытается атаковать союзников
- Исправлено поведение `auto_attack.valid_targets`
- Добавлен цвет в таблицу очков и модели
- Исправлено строительство за границами карты

## 0.1.1-beta

- QuickStart теперь корректно сохраняется в конфигурации,
- Максимальное количество еды показываемое в приложении теперь учитывает только активные сущности (как и должно),
- Уничтожение союзных сущностей не приносит очков