# qa_python

В этом файле описаны тесты которые удалось реализовать в проекте.
Всего в проекте удалось реализовать 13 тестов.
Есть негативные и позитивные тесты, 3 раза использована параметризация, задействовано 7 фикстур.

Тест 1 Проверка добавления книг
Позитивная проверка метода add_new_book с использованием параметризации и фикстуры collector

Тест 2 Нельзя добавить одну и ту же книгу дважды
Негативная проверка метода add_new_book - пытались дважды добавить книгу 'The Great Gatsby' в словарь books_rating. Использовали фикстуры collector и new_book

Тест 3 Проверка добавления рейтинга книг
Позитивная проверка метода set_book_rating c использованием параметризации и фикстуры collector

Тест 4 Нельзя выставить рейтинг книге, которой нет в списке
Негативная проверка метода set_book_rating - пытались выставить рейтинг книге 'Fight Club', которой не было в словаре books_rating. Использовали фикстуры collector и new_book

Тест 5 Нельзя выставить рейтинг больше 10
Негативная проверка метода set_book_rating - пытались выставить книге 'The Great Gatsby' рейтинг 11. Использовали фикстуры collector и new_book

Тест 6 Нельзя выставить рейтинг меньше 1
Негативная проверка метода set_book_rating - пытались выставить книге 'Of Mice and Men' рейтинг 0. Использовали фикстуры collector и new_book

Тест 7 Проверка получения рейтинга книги по ее имени
Позитивная проверка метода get_book_rating. Использовали фикстуры collector и new_book

Тест 8 Проверка вывода списка книг с определенным рейтингом
2 позитивные и 1 негативная проверка метода get_books_with_specific_rating. Использовали фикстуры collector, new_books и set_new_books.
В случае позитивной проверки пытались вывести список книг с рейтингом 8(1й тест) и рейтином 7(2й тест).
В случае негативной проверки(последний тест), пытались вывести список книг с несуществующим рейтингом 3(3й тест).

Тест 9 Проверка получения словаря books_rating
Позитивная проверка метода get_books_rating с использованием параметризации и фикстуры collector

Тест 10 Проверка добавления книги в избранное
Позитивная проверка метода get_list_of_favorites_books c использованием фикстур collector и add_to_favorite

Тест 11 Нельзя добавить книгу в избранное, если её нет в словаре books_rating
Негативная проверка метода get_list_of_favorites_books - передавали неверный параметр('The Great Gatsby'), которого не было в словаре books_rating. Использовали фикстуры collector и new_book_2

Тест 12 Проверка удаления книги из избранного
Позитивная проверка метода delete_book_from_favorites c использованием фикстурcollector и new_book

Тест 13 Проверка получения списка Избранных книг
Позитивная проверка метода get_list_of_favorites_books с использованием фикстур collector, new_books, favorite_books
