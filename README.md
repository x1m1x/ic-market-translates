# Ic-Market

# Памятка для переводчика

В документе используется формат JSON.

## Правила синтаксиса JSON

- Данные записываются в виде пар "имя/значение"
- Данные разделяются запятыми
- В фигурных скобках записываются объекты
- В квадратных скобках записываются массивы
- Данные JSON – Имя и значение
- Данные JSON записываются в виде пар "имя/значение".

Пара "имя/значение" состоит из имени поля (в двойных кавычках), за которым ставится двоеточие, за которым идет значение.

Для корректного перевода необходимо скопировать файл для каждого языка и изменить только значения, не затрагивая ключи.

## Как ориентироваться в файле

Все слова на исходном (русском) языке выписаны исходя из содержания страниц сайта. Все страницы можно просмотреть в [дизайне по ссылке](https://www.figma.com/file/u582eC05DAJUP3TznAFzXu/Infinity-Construction-%2F-Web-Design?node-id=1436%3A4833https://www.figma.com/file/u582eC05DAJUP3TznAFzXu/Infinity-Construction-%2F-Web-Design?node-id=1436%3A4833)

Для облегчения работы с файлом локализации все ключи имеют в себе семантические префиксы/cуффиксы. Они подсказывают где и как используется конкретный ключ.

Список возможных префиксов/cуффиксов:

- ui_ - пользовательский интерфейс, слово является статичным и используется в интерфейсе приложения
- ui_page - страница, слово используется один раз на конкретной страницы. После префикса указывается название этой страницы
- ui_component - компонент, слово используется в нескольких местах приложения
- ui_component_modal - слово используется в модальном окне
- ui_input - поле для ввода чего-либо, слово используется в форме для ввода
- ui_errors / error_code - текст ошибки
- reference_ / enum_ - справочник значений, динамическое значение которое может использоваться как значение поля, статус чего-либо
- _placeholder - слово указывается в форме для ввода как значение по умолчанию, пропадает когда пользователь начинает вводить свое значение
- _btn - кнопка, слово используется в кнопке
- _title - заголовок, слово используется как заголовок страницы/блока
- _label - название формы для ввода или название компонета
- _description - описание формы для ввода

Примечания:

- Значение, ключ которых начинается со знака "@" следует игнорировать.
- В словах могут встречаться записи вроде "{count}" или "{tab}", они обозначают динамическое значение которое будет вставляться во время работы. При переводе нужно учесть в каком месте подставляется значение. Например перевод "Найдено {count} объявлений" на английский должен выглядеть примерно как "{count} adverts found"
