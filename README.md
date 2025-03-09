# **🚀 Git: подробный конспект и команды**

Git — распределённая система контроля версий, помогающая отслеживать изменения в коде, управлять проектами и взаимодействовать с другими разработчиками.

## **⚡ Основы Git**

- **Репозиторий (repository)** — хранилище всех файлов и их истории изменений.
- **Коммит (commit)** — фиксирует изменения в истории репозитория.
- **Ветви (branches)** — параллельные линии разработки проекта.

## **💻 Основные команды**

### 🔹 **Инициализация репозитория**
```
git init
```
### 🔹 **Клонирование репозитория**

git clone [ссылка на репозиторий]

### 🔹 **Проверка состояния**
```
git status
```
### 🔹 **Добавление файлов**

Добавить один файл:
```
git add filename
```
Добавить все файлы:
```
git add .
```
### 🔹 **Создание коммита**
```
git commit -m "Описание изменений"
```
### 🔹 **Просмотр истории коммитов**
```
git log
```
Упрощенный просмотр:
```
git log --oneline
```
## 🔄 **Работа с ветками**

### 🔹 **Создание новой ветки**
```
git branch название_ветки
```
### 🔹 **Переключение на ветку**
```
git checkout название_ветки
```
Создание и переход на новую ветку одновременно:
```
git checkout -b название_ветки
```
### 🔹 **Слияние веток**

Перейдите на ветку, в которую хотите внести изменения, и выполните:
```
git merge название_ветки
```
### 🔹 **Удаление ветки**
```
git branch -d название_ветки
```
## **📡 Работа с удалёнными репозиториями**

### 🔹 **Добавление удалённого репозитория**
```
git remote add origin [ссылка]
```
### 🔹 **Отправка изменений в удалённый репозиторий**
```
git push -u origin название_ветки
```
### 🔹 **Получение изменений с удалённого репозитория**

Получение и слияние:
```
git pull
```
Только получение изменений:
```
git fetch
```
## 🛠️ **Отмена изменений**

Отмена изменений в рабочем каталоге:
```
git checkout -- filename
```
Отмена добавления файла (из staged в unstaged):
```
git reset filename
```
Отмена последнего коммита (сохранение изменений):
```
git reset --soft HEAD~1
```
Отмена последнего коммита (удаление изменений):
```
git reset --hard HEAD~1
```
## 🚨 **Решение конфликтов**

При слиянии веток может произойти конфликт:

Исправьте конфликт вручную в файлах.

После исправления добавьте файлы и создайте новый коммит.
```
git add filename
git commit -m "исправлен конфликт"
```
## 🧭 **Полезные команды**

Показать различия между коммитами:
```
git diff commit1 commit2
```
Посмотреть удалённые репозитории:
```
git remote -v
```
Удалить удалённый репозиторий из списка:
```
git remote remove origin
```
## 📌 **Итог**
Используя эти команды, вы сможете эффективно контролировать версии ваших проектов и взаимодействовать с командой.
