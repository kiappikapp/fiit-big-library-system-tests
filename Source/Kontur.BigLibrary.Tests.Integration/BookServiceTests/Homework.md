Напишите интеграционные тесты на BookService.

На лекции мы написали тест ***SaveBookAsync_ReturnSameBook_WhenSaveCorrectBook***. 
Допишите проверки в Assert, чтобы точно быть уверенными, что интеграция работает корректно. Нужно проверить все оставшиеся параметры книги.

В этом тесте происходит реальное взаимодействие с БД.
Но иногда интеграционные тесты на взаимодействие между классами проще писать с замоканной БД.
Для этого напишите тест в классе ***BookServiceMockTest***.
Для регистрации зависимостей используйте DI-контейнер с помощью [Microsoft.Extensions.DependencyInjection](https://learn.microsoft.com/ru-ru/dotnet/core/extensions/dependency-injection).
Для написания моков используйте [NSubstitute](https://nsubstitute.github.io/).

Помните про правила написания тестов, которые обсуждались на прошлых лекциях.