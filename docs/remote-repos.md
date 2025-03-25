# 🌐 Работа с удаленными репозиториями

## 📡 Основные операции

### Подключение к удаленному репозиторию
```bash
# Добавить удаленный репозиторий
git remote add origin https://github.com/username/repo.git

# Просмотр списка удаленных репозиториев
git remote -v

# Изменить URL удаленного репозитория
git remote set-url origin https://github.com/username/repo.git
```

### Синхронизация с удаленным репозиторием

```bash
# Получить изменения с удаленного репозитория
git fetch origin

# Получить изменения и слить их с локальной веткой
git pull origin main

# Отправить изменения в удаленный репозиторий
git push origin main

# Отправить все ветки
git push --all origin
```

## 🔑 Настройка SSH-доступа

1. **Генерация SSH-ключа:**
```bash
ssh-keygen -t ed25519 -C "ваш@email.com"
```

2. **Добавление публичного ключа на GitHub:**
   - Скопируйте содержимое файла `~/.ssh/id_ed25519.pub`
   - Перейдите в настройки GitHub → SSH and GPG keys
   - Нажмите "New SSH key" и вставьте ключ

## 👥 Совместная работа

### Форки (Forks)
1. Создайте форк репозитория на GitHub
2. Клонируйте свой форк:
```bash
git clone git@github.com:ваш-username/repo.git
```

### Pull Requests
1. Создайте новую ветку:
```bash
git checkout -b feature/новая-функция
```

2. Внесите изменения и отправьте их:
```bash
git push origin feature/новая-функция
```

3. Создайте Pull Request на GitHub

[⬅️ Назад к ветвлению](branching.md) | [Вперед к слиянию и конфликтам ➡️](merging.md) 