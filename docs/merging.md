# 🔄 Слияние и разрешение конфликтов

## 📝 Виды слияния

### Fast-forward слияние
```bash
# Простое слияние без создания коммита слияния
git merge feature-branch
```

### Слияние с созданием коммита
```bash
# Создает новый коммит слияния
git merge --no-ff feature-branch
```

## ⚠️ Конфликты слияния

### Когда возникают конфликты?
- Изменения одних и тех же строк в разных ветках
- Удаление файла в одной ветке и его изменение в другой
- Конфликты переименования

### Разрешение конфликтов

1. **Определение конфликтующих файлов:**
```bash
git status
```

2. **Структура конфликта:**
```text
<<<<<<< HEAD
Ваши изменения
=======
Изменения из другой ветки
>>>>>>> feature-branch
```

3. **Способы разрешения:**
   - Ручное редактирование файлов
   - Использование инструментов:
     ```bash
     git mergetool
     ```

4. **Завершение слияния:**
```bash
git add .
git commit -m "Разрешение конфликтов слияния"
```

## 🛠 Инструменты для разрешения конфликтов

- **Visual Studio Code**
- **GitKraken**
- **Meld**
- **Beyond Compare**

## 💡 Лучшие практики

1. Регулярно синхронизируйтесь с основной веткой
2. Делайте небольшие, атомарные коммиты
3. Используйте осмысленные сообщения коммитов
4. Проверяйте изменения перед слиянием

[⬅️ Назад к удаленным репозиториям](remote-repos.md) | [Вперед к Git Flow ➡️](git-flow.md) 