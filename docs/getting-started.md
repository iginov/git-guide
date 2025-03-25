# 🚀 Начало работы с Git

## Установка Git

### Windows
1. Скачайте установщик с [официального сайта](https://git-scm.com/)
2. Запустите установщик и следуйте инструкциям
3. Проверьте установку командой:
```bash
git --version
```

### Linux
Установка через терминал:
```bash
# Ubuntu/Debian
sudo apt-get update
sudo apt-get install git

# Fedora
sudo dnf install git
```

### macOS
1. Установите через Homebrew:
```bash
brew install git
```

## ⚙️ Первоначальная настройка

Настройка имени пользователя и email:

```bash
git config --global user.name "Ваше Имя"
git config --global user.email "ваш@email.com"
```

## 📝 Создание первого репозитория

```bash
# Создание нового репозитория
git init

# Добавление файлов в индекс
git add .

# Создание первого коммита
git commit -m "Инициализация проекта"
```

[⬅️ Вернуться к содержанию](../README.md) | [Вперед к основным командам ➡️](basic-commands.md) 