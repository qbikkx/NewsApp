# KeepSolidOne

Current home work:

Все задание делать в том же проекте, который вы создали на первом задании, и залили в гит на втором (НЕ общий репозиторий, а ваш личный.)
Задание делать в отдельной ветке, после чего слить ее с Master.

Базовый уровень:
Сделать в приложении два Activity. В первом Activity добавить поле для ввода и две кнопки.

Кнопка "Очистить" очищает поле от текста. Кнопка "Отправить" - отправляет введенный текст из текстового поля на второе активити.
Второе активити должно принимать текст из первого и выводить его как статичный текст. На втором активити так же присутствуют две кнопки. Одна "Подтвердить", вторая "Отклонить".

По нажатию на "подтвердить" происходит возврат на предыдущее активити, при этом поле для ввода на нем очищается.

По нажатию на "Отклонить" происходит возврат на предыдущее активити, введенный в поле для ввода текст остается на месте.

По желанию можно сопроводить возврат на активити Toast-сообщением, которео будет уведомлять о том, подтвердил пользователь текст, или нет. 
Все поля для вода должны проверяться на пустоту. Если поле пустое - отправку и открытие второго активити НЕ производить. Также везде должны быть проверки на null (интент в onActivityResult может быть null).

Усложненный уровень:
То же самое что в базовом, НО:
 - Поле для ввода на первом активити должно быть настроено для ввода Email. В нем также должна быть введена подсказка (xml - android:hint) "Введите email адррес".
 - На первом активити также есть чекбокс (галочка, Checkbox) с подписью "Разрешить". Если галочки нет - кнопка "Отправить" должна быть неактивной. Если есть - активной.
 - По нажатию "Отправить" на первом активити проверяем не только пустоту поля, но и то, введен ли в поле настоящий Email (Можно проверить только по наличию в введенном тексте символа "@").
 - Во втором активити так же выводим введенный email адрес.
 - Во втором активити по нажатию на "подтвердить" - запускаем неявным интентом отправку email сообщения на введенный адрес, выводим Toast сообщение с текстом "Отправка сообщения..." и закрываем второе активити.
 - По нажатию "Отклонить" возвращаемся на предыдущее активити БЕЗ очистки полей и выводим Toat с текстом "Пользователь не подтвердил адрес".
 Все типы заданий делаем с проверками. Используем удобные для вас менеджеры разметки.