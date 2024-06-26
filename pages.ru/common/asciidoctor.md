# asciidoctor

> Преобразователь AsciiDoc файлов в другие форматы для публикации.
> Больше информации: <https://docs.asciidoctor.org>.

- Преобразовать данный `.adoc` файл в HTML (формат на выходе по умолчанию):

`asciidoctor {{путь/до/файла.adoc}}`

- Преобразовать данный `.adoc` файл в HTML и привязать к таблице стилей CSS:

`asciidoctor -a stylesheet {{путь/до/таблицы-стилей.css}} {{путь/до/файла.adoc}}`

- Преобразовать данный `.adoc` файл во встраиваемый HTML, убрав всё кроме самого текста:

`asciidoctor --embedded {{путь/до/файла.adoc}}`

- Преобразовать данный `.adoc` файл в PDF с помощью библиотеки `asciidoctor-pdf`:

`asciidoctor --backend {{pdf}} --require {{asciidoctor-pdf}} {{путь/до/файла.adoc}}`
