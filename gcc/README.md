# Сборка, запуск и тестирование проекта

Сборка проекта, исходники которого находятся в `CODE_DIR`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc build
```

---

Компиляция `main.cpp`, который находится в `CODE_DIR`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc compile-main
```

---

Удалить директорию `build` (в которой находятся скомпилированные исходники):

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc clear
```

---

Запуск программы:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc run-main
```

---

Запуск тестов:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc run-tests
```

---

> `CODE_DIR` – это путь до папки с проектом\
> `-C <path>` – путь до файла `Makefile`
