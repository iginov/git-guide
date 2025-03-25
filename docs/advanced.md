# 🚀 Продвинутые техники Git

## 🔍 Поиск и отладка

### Git Bisect
```bash
# Запуск бинарного поиска
git bisect start

# Отметить текущий коммит как плохой
git bisect bad

# Отметить старый коммит как хороший
git bisect good <commit-hash>

# Завершить поиск
git bisect reset
```

### Git Blame
```bash
# Просмотр авторов строк файла
git blame filename.txt

# С указанием диапазона строк
git blame -L 10,20 filename.txt
```

## 🧹 Обслуживание репозитория

### Очистка и оптимизация
```bash
# Очистка неиспользуемых объектов
git gc

# Проверка целостности репозитория
git fsck

# Сжатие репозитория
git prune
```

### Работа с подмодулями
```bash
# Добавление подмодуля
git submodule add <repository-url>

# Инициализация подмодулей
git submodule init

# Обновление подмодулей
git submodule update
```

## 🎯 Продвинутое использование reset

```bash
# Мягкий reset (сохраняет изменения в индексе)
git reset --soft HEAD~1

# Смешанный reset (по умолчанию)
git reset HEAD~1

# Жесткий reset (удаляет все изменения)
git reset --hard HEAD~1
```

## 📌 Cherry-pick

```bash
# Перенос отдельного коммита
git cherry-pick <commit-hash>

# Перенос нескольких коммитов
git cherry-pick <commit-hash-1> <commit-hash-2>

# Перенос без создания коммита
git cherry-pick -n <commit-hash>
```

[⬅️ Назад к Git Flow](git-flow.md) | [Вперед к лучшим практикам ➡️](best-practices.md) 