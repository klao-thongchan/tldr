# cabal

> Интерфейс командной строки для инфраструктуры пакетов Haskell (Cabal).
> Управление Haskell-проектами и Cabal-пакетами из репозитория Hackage.
> Больше информации: <https://cabal.readthedocs.io/en/latest/getting-started.html>.

- Искать и вывести список пакетов из Hackage:

`cabal list {{строка_поиска}}`

- Показать информацию о пакете:

`cabal info {{имя_пакета}}`

- Скачать и установить пакет:

`cabal install {{имя_пакета}}`

- Создать новый Haskell-проект в текущей папке:

`cabal init`

- Собрать проект в текущей папке:

`cabal build`

- Запустить тесты из проекта в текущей папке:

`cabal test`
