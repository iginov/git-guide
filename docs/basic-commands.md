# 🛠 Основные команды Git

## 📋 Основные операции

### Создание и клонирование репозиториев
```bash
# Создать новый репозиторий
git init

# Клонировать существующий репозиторий
git clone <url-репозитория>
```

### Работа с изменениями

#### Просмотр статуса
```bash
# Показать статус рабочей директории
git status

# Показать изменения в файлах
git diff
```

#### Добавление файлов
```bash
# Добавить все файлы
git add .

# Добавить конкретный файл
git add имя-файла

# Добавить все файлы определенного типа
git add *.md
```

#### Создание коммитов
```bash
# Создать коммит с сообщением
git commit -m "Ваше сообщение"

# Добавить файлы и создать коммит одной командой
git commit -am "Ваше сообщение"
```

## 📜 История изменений

### Просмотр истории
```bash
# Показать историю коммитов
git log

# Показать историю в компактном виде
git log --oneline

# Показать историю с графом веток
git log --graph --oneline --all
```

## 🔄 Отмена изменений

```bash
# Отменить изменения в рабочей директории
git checkout -- <файл>

# Отменить изменения в индексе
git reset HEAD <файл>

# Создать новый коммит, отменяющий изменения предыдущего
git revert <хеш-коммита>
```

## 🏷 Работа с метками (тегами)

```bash
# Создать новую метку
git tag v1.0.0

# Создать аннотированную метку
git tag -a v1.0.0 -m "Версия 1.0.0"

# Показать список меток
git tag
```

[⬅️ Назад к началу работы](getting-started.md) | [Вперед к ветвлению ➡️](branching.md) 