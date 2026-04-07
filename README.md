# 🩺 Дневник давления — PWA

Приложение для ежедневного трекинга артериального давления.

## Структура файлов

```
index.html      ← главная страница
manifest.json   ← PWA манифест
sw.js           ← Service Worker (офлайн)
icons/
  icon-192.png
  icon-512.png
```

## Деплой на GitHub Pages (5 минут)

### 1. Создай репозиторий
- Зайди на github.com → New repository
- Имя: `davlenie` (или любое)
- Сделай **Public**
- Нажми Create repository

### 2. Загрузи файлы
```bash
git init
git add .
git commit -m "feat: blood pressure PWA"
git branch -M main
git remote add origin https://github.com/ТВО_ИМЯ/davlenie.git
git push -u origin main
```

### 3. Включи GitHub Pages
- Settings → Pages → Source: **Deploy from branch**
- Branch: `main` / `/ (root)` → Save
- Через ~1 минуту сайт будет на: `https://ТВО_ИМЯ.github.io/davlenie`

### 4. Установи как приложение на Android
- Открой ссылку в **Chrome**
- Меню (⋮) → **"Добавить на главный экран"**
- Готово — иконка появится как обычное приложение

## Функции

- ✅ Ввод систолического и диастолического давления
- 📋 Журнал всех записей с категориями (Норма / Повышенное / Гипертония 1° / 2°)
- 📈 График последних 14 дней
- 📊 Сводная статистика (среднее, макс, мин)
- 📄 Экспорт CSV для врача
- 📶 Работает офлайн (Service Worker)
- 💾 Данные хранятся локально в браузере

## Напоминание

Будильник на 7:30 уже поставлен через Claude.
