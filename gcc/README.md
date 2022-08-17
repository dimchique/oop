# Сборка, запуск и тестирование проекта

Пример cборки проекта, исходники которого находятся в `CODE_DIR`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc build
```

Запуск программы:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc run-main
```

Запуск тестов:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc run-tests
```
