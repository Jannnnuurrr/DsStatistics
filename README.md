import pandas as pd
# Ваш новый набор данных
new_data = {
    'Имя': ['Алиса', 'Боб', 'Чарли', 'Дэвид', 'Ива́н'],
    'Чистая_стоимость_в_миллиардах': [90, 75, 60, 45, 30],
    'Возраст': [35, 42, 50, 28, 55],
    'Отрасль': ['Технологии', 'Финансы', 'Здравоохранение', 'Технологии', 'Развлечения'],
    'Страна': ['Канада', 'Соединенные Штаты', 'Соединенное Королевство', 'Австралия', 'Бразилия'],
    'Источник_богатства': ['Программное обеспечение', 'Инвестиции', 'Фармацевтика', 'Электронная коммерция', 'Медиа']
}
# Создание нового датафрейма
new_health_data = pd.DataFrame(new_data)
# Установка опций для отображения всех столбцов и строк
pd.set_option('display.max_columns', None)
pd.set_option('display.max_rows', None)
# Вывод статистического описания нового набора данных
print(new_health_data.describe())

