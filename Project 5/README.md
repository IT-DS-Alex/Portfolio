# Анализ рынка игровой индустрии
Анализ исторических данных по продажам игр на различных платформах. Необходимо выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании на 2017 год.

## Описание данных
• Name — название игры

• Platform — платформа

• Year_of_Release — год выпуска

• Genre — жанр игры

• NA_sales — продажи в Северной Америке

• EU_sales — продажи в Европе

• JP_sales — продажи в Японии

• Other_sales — продажи в других странах

• Critic_Score — оценка критиков

• User_Score — оценка пользователей

• Rating — рейтинг от организации ESRB

### Вывод подготовка данных
1. Привели название столбцов к нижнему регистру.
2. Избавились от пропусков: удалили в столбцах - там где их очень мало.
3. Добавили отдельный столбец'sum_sales'.
4. Заменили тип данных.

### Исследовательский анализ данных

![image](https://github.com/IT-DS-Alex/Portfolio/assets/140064630/19b6939e-6ea9-4222-b09e-735cafeff6e8)

#### Вывод: 
Самые популярные жанры ожидаемо - шутеры, спорт. Хуже всего продаются приключения и симуляторы.

### Общий вывод(Планируемая кампания на 2017-й):
1.Так как мы заметили, что жизненный цикл игр -10 лет и по графикам, что все игры на данный момент находятся на стадии спада своей популярности. Считаем, что здесь наибольшая вероятность "оживить" продажу можно - платформу PS4 (дата выхода 2013). По свежести дате выхода предыдущие игры X360, PS3 уже старые.

2.Предлагаем принять разные стратегии по повышению продаж в регионах в зависимости от актуальных параметров игр, т.е. использовать портреты средне-статистического пользователя каждого региона.Принять важное замечание, что больше половины продаж сделано в Северной Америке.

3.Предлагаем выпустить новую игру, например, PS5 на базе платформы X360 и PS4 c жанром "Action" и "Sports", рейтингом "Для взрослых" и запустить продажу в Северной Америке и Европе. Для Японии выпустить больше игр на платформе 3DS, жанру Role-Playing, рейтингу "Для всех", но при этом использовать рекламные акции о популярных платформах в других регионах для ознакомления.
