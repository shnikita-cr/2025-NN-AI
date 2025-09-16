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

```bash
# Установка virtualenv
python -m pip install virtualenv

# Создание окружения
python -m virtualenv myenv

# Активация окружения
# Windows:
myenv\Scripts\activate
# macOS/Linux:
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
# Экспорт установленных пакетов
pip freeze > requirements.txt

# Установка из requirements.txt
pip install -r requirements.txt
```