# HTTP-сервер своими руками
Ограничения:
* запрещено использовать модуль http
* запрещено пользоваться синхронными версиями функций (с **Sync**) на конце


## Уровень сложности 0
(Этот уровень сложности задания присылать не надо - вы получите "расширенную версию задания" после второй лекции по потокам во вторник, ее уже надо будет присылать и будет описан требуемый формат)

Реализовать HTTP-сервер, который слушает порт 3000, или указанный в переменной окружении PORT и умеет следующее:

1. Выводит на консоль все полученные заголовки в формате ключ-значение
2. При обращении допустим к `http://localhost:3000/foo.html` если в папке `static` проекта есть файл `foo.html` - он будет корректно работать
3. Скрипт корректно работает для бинарных файлов (к примеру картинок)
4. Скрипт корректно возвращает `404` если файл отсутствует в файловой системе
5. Скрипт корректно возвращает `400` если файл недоступен на чтение (привет правам доступа файловой системы)

Спецификация протокола HTTP для тех кто с ней не знаком: 
https://habrahabr.ru/post/215117/
https://www.ietf.org/rfc/rfc2616.txt