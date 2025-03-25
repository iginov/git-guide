# ⚙️ Настройка Git

## 🔧 Основные настройки

### Глобальная конфигурация
```bash
# Установка имени и email
git config --global user.name "Ваше Имя"
git config --global user.email "ваш@email.com"

# Настройка редактора
git config --global core.editor "code --wait"

# Настройка инструмента слияния
git config --global merge.tool vscode
```

### Локальная конфигурация проекта
```bash
# Настройки только для текущего репозитория
git config user.name "Проектное Имя"
git config user.email "project@email.com"
```

## 🎨 Цветовое оформление

```bash
# Включение цветового оформления
git config --global color.ui true

# Настройка цветов для различных команд
git config --global color.status.changed "yellow"
git config --global color.status.untracked "red"
```

## 📝 Файлы конфигурации

### Уровни конфигурации
1. **Системный** (`/etc/gitconfig`)
2. **Глобальный** (`~/.gitconfig`)
3. **Локальный** (`.git/config`)

### Просмотр настроек
```bash
# Все настройки
git config --list

# Конкретная настройка
git config user.name
```

## 🔑 Настройка аутентификации

### SSH-ключи
```bash
# Генерация ключа
ssh-keygen -t ed25519 -C "ваш@email.com"

# Проверка подключения
ssh -T git@github.com
```

### Credential Helper
```bash
# Windows
git config --global credential.helper wincred

# macOS
git config --global credential.helper osxkeychain

# Linux
git config --global credential.helper cache
```

[⬅️ Назад к лучшим практикам](best-practices.md) | [Вперед к FAQ ➡️](faq.md) 