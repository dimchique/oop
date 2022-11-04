# Сборка и запуск проекта

Ссылка на скачивание докера <https://www.docker.com/products/docker-desktop>

`CODE_DIR` – директория, в которой находятся исходники проекта\
`-C <path>` – директория, в которой находится `Makefile`

## Команды

Собрать проект, исходники которого находятся в `CODE_DIR`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc build
```

или, если не установлен `make`, то

```bash
CODE_DIR=/Users/my-user/Desktop/my-project docker-compose run --rm gcc-cmake bash -c "cmake -S . -B build && make -C build"
```

(команда после `CODE_DIR=<path>` взята из `Makefile`)

---

Скомпилировать `main.cpp`, который находится в `CODE_DIR`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc compile-main
```

---

Удалить директорию `build` (в которой находятся скомпилированные исходники):

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc clear
```

---

Запустить скомпилированную точку входа `main.cpp`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc run-main
```

---

Запустить скомпилированную точку входа `tests.cpp`:

```bash
CODE_DIR=/Users/my-user/Desktop/my-project make -C /Users/my-user/Desktop/oop/gcc run-tests
```
