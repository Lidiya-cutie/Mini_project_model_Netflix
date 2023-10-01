# Построение рекомендательной системы content-based model на основе популярности
Допустим мы получили задание построить рекомендательную систему на основе контента, где необходимо:

* Для каждого продукта создать характеризующие его признаки.
* Найти показатель близости между всеми продуктами.
* Порекомендовать пользователю продукты, которые показывают наибольшую близость с теми продуктами, которые он высоко оценил.

Реализуем подобную рекомендательную систему на практике. Будем работать с [датасетом](), содержащим информацию об оценивании фильмов на платформе Netflix.

Признаки в данных:

* *show_id* — id фильма,
* *type* — его тип (фильм или сериал),
* *title* — название,
* *director* — режиссер,
* *cast* — актерский состав,
* *country* — страна,
* *date_added* — дата добавления,
* *release_year* — год выхода на экраны,
* *rating* — рейтинг,
* *duration* — продолжительность,
* *listened_in* — жанр(-ы),
* *description* — описание.


Выводы по данному проекту:

* мы можем использовать фильтрацию по контенту, чтобы создавать рекомендации из аналогичных элементов;
* у нас получилось рекомендовать пользователю продукты, которые показывают наибольшую близость с теми продуктами, которые пользователь высоко оценил;
* мы не сможем порекомендовать продукты другого жанра или контента, если пользователь сам не отметит подобные фильмы как понравившиеся.
