# Установка Python 3.10 и настройка окружения

## Установка Python 3.10

1. Скачайте установщик с официального сайта:
    - Windows: https://www.python.org/downloads/release/python-3100/
    - macOS: Используйте Homebrew: `brew install python@3.10`
    - Linux: `sudo apt install python3.10`

2. При установке отметьте опцию "Add Python to PATH"

3. Проверьте установку:
   ```bash
   python --version
   ```

## Создание виртуального окружения

Все команды далее стоит выполнять в корневой папке проекта, в данном случае `2025-NN-AI`

```bash
# Установка virtualenv
python -m pip install virtualenv

# Создание окружения
python -m virtualenv myenv
# myenv - имя для папки с виртуальным окружением, выбирается пользователем
```

```bash
# Активация окружения
# только для Windows:
myenv\Scripts\activate
```

```bash
# Активация окружения
# только для macOS/Linux:
source myenv/bin/activate
```

## Установка библиотек через pip

```bash
# Формат
pip install [name] 

# Пример
pip install jupyter
```

## Сохранение зависимостей

```bash
# Установка зависимостей из requirements.txt
pip install -r requirements.txt #  общие пакеты
pip install -r lab1\requirements.txt # пакеты для лабораторной 1
```