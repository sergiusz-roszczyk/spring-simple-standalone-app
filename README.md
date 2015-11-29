# Przykładowa aplikacja wiersza poleceń z kontekstem Spring
Jest to przykładowa implementacja kontekstu Spring, bez użycia plików XML. Wyłącznie z użyciem annotacji Javy.

Przygotowana została z myślą o posiadaczach Raspberry Pi, którzy chcieliby tworzyć aplikacje odpowiadające
na zdarzenia zewnętrzne (np. przy użyciu PI4J), a jednocześnie korzytać z możliwości wstrzykiwania zależności
i wszystkie inne korzyści, które daje ze sobą Spring.

## Uruchamianie

Aplikację można uruchomić wydając poniższe polecenie w katalogu projektu:

java -jar target/spring-simple-standalone-app.jar

Java potrafi skonsumować dużą ilość pamięci. Jeśli Twoja aplikacja nie generuje dużych ilości obiektów
i chcesz ograniczyć zajmowaną pamięć, umożliwiając współistnienie z innymi, niezależnymi procesami
możesz ograniczyć użycie pamięci Heap. Poniższy przykład ogranicza rozmiar heapa do 128 MB.

java -Xmx128m -jar target/spring-simple-standalone-app.jar

# Sample Spring Context CLI (Command Line Interface) Application

This is a sample implementation of pure Java based Spring Context configuration. No XML files, only annotations.

It was prepared with Raspberry Pi owners in mind, who want to create apps responding to external events (ie. using PI4J),
meanwhile use all benefits of Spring and dependency injection.

## Running app

Application can be run by running the following command from project directory:

java -jar target/spring-simple-standalone-app.jar

Java can consume a lot of memory. If your app is doesn't create a lot of objects
and you want to keep memory usage under control, enabling other, independent apps running you can limit heap usage.
Sample below limits Heap memory to 128 MB.

java -Xmx128m -jar target/spring-simple-standalone-app.jar