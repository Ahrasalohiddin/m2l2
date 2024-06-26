# покемоны
# телеграм боту нужно написать команду go.
Мой проект представляет собой симуляцию игры с покемонами, где каждый покемон принадлежит определенному тренеру и может выполнять различные действия, такие как атака и кормление. Проект включает использование API для получения информации о покемонах. Давайте рассмотрим каждый элемент более подробно.

Классы и методы
1. Класс Pokemon
Базовый класс, представляющий покемона. Он содержит основную информацию и функциональность, такую как получение изображения и имени покемона из API.

Атрибуты:

pokemon_trainer: имя тренера покемона.
pokemon_number: случайный номер покемона.
img: URL изображения покемона, полученный через API.
name: имя покемона, полученное через API.
last_feed_time: время последнего кормления.
Методы:

__init__: инициализация объекта.
feed: метод для кормления покемона, увеличивающий его здоровье при соблюдении интервала времени.
get_img: получение URL изображения покемона через API.
get_name: получение имени покемона через API.
info: возвращает информацию о покемоне.
show_img: возвращает URL изображения покемона.
attack: метод для атаки другого покемона.
2. Классы-наследники Wizard и Fighter
Эти классы представляют покемонов особых типов и добавляют или изменяют некоторые функциональности базового класса Pokemon.

Класс Wizard:

Переопределяет метод feed, увеличивая здоровье на большее количество единиц.
Класс Fighter:

Переопределяет метод attack, добавляя возможность использовать супер-атаку с увеличенной силой.
Переопределяет метод feed, уменьшая интервал между кормлениями.
Особенности проекта
Использование API:

Для получения информации о покемонах используется PokeAPI. Это позволяет получать актуальные данные, такие как имя и изображение покемона, основываясь на случайно сгенерированном номере.
Кормление покемонов:

Покемонов можно кормить, что увеличивает их здоровье. Для этого учитывается интервал времени между кормлениями, что предотвращает чрезмерное увеличение здоровья за короткий промежуток времени.
Атака:

Покемоны могут атаковать друг друга. Успешная атака уменьшает здоровье противника, а в случае победы здоровье противника обнуляется.
Типы покемонов:

Wizard имеет улучшенные способности в кормлении.
Fighter обладает возможностью использовать супер-атаку и чаще кормится.
Потенциальные улучшения
Добавление новых типов покемонов с уникальными способностями.
Расширение функционала атаки, включающее больше видов атак и стратегий.
Интеграция с интерфейсом пользователя для удобного взаимодействия.
Добавление хранения данных о покемонах и их тренерах для долговременного использования.
Мой проект интересен и предоставляет основу для дальнейшего расширения и улучшения, предлагая увлекательный опыт взаимодействия с покемонами.Ж
