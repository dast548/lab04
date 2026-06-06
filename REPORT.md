# Отчёт по лабораторной работе №3

## Тема
Изучение систем автоматизации сборки проекта на примере CMake.

## Выполнение

### Подготовка
- Создан репозиторий lab03 на GitHub
- Установлен cmake и g++
- Скопированы исходные файлы из tp-labs/lab03

### Задание 1 — formatter_lib
Создан `formatter_lib/CMakeLists.txt` для сборки статической библиотеки formatter.

### Задание 2 — formatter_ex_lib
Создан `formatter_ex_lib/CMakeLists.txt` для библиотеки formatter_ex,
которая использует библиотеку formatter через target_link_libraries.

### Задание 3 — приложения
Созданы CMakeLists.txt для:
- `hello_world_application` — использует библиотеку formatter_ex
- `solver_application` — использует formatter_ex и solver_lib

Также исправлена ошибка в solver.cpp: заменён `std::sqrtf` на `std::sqrt`
и добавлен заголовочный файл `<cmath>`.

### Сборка проекта
```bash
mkdir build && cd build
cmake ..
cmake --build .
```

## Вывод
В ходе работы изучена система сборки CMake. Научился создавать CMakeLists.txt
для статических библиотек и исполняемых файлов, настраивать зависимости
между библиотеками через target_link_libraries.
cmake --build.
```

## Вывод
В ходе работы изучена система сборки CMake. Научился создавать CMakeLists.txt
для статических библиотек и исполняемых файлов, настраивать зависимости
между библиотеками через target_link_libraries.
