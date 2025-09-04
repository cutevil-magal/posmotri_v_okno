# Видеопоиск "Посмотри в окно"

**Адаптивный видеопоиск с современным интерфейсом**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/ru/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/ru/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/ru/docs/Web/JavaScript)
[![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://figma.com)

---

## 📖 О проекте

Я разработала современный видеопоиск "Посмотри в окно" с адаптивным интерфейсом и плавными взаимодействиями. Проект представляет собой полнофункциональное веб-приложение для поиска и просмотра видеоконтента с акцентом на пользовательский опыт.

### 🎯 Ключевые особенности

- **Адаптивная сетка карточек** с поддержкой lazy loading
- **Динамическая подгрузка контента** по требованию
- **Поисковая система** с мгновенными результатами
- **Система обработки ошибок** и состояний загрузки
- **Оптимизированный видео-плеер** с контролами

### 🛠 Технологический стек

**Frontend:**
- HTML5 (семантическая разметка)
- CSS3 (Grid, Flexbox, анимации)
- Vanilla JavaScript (ES6+)
- REST API интеграция

**Инструменты:**
- Figma для работы с дизайн-макетом
- Git для контроля версий
- GitHub Pages для деплоя

---

## 🚀 Быстрый старт

### Посмотреть онлайн

🌐 **[Живая демо-версия](https://cutevil-magal.github.io/posmotri_v_okno/)**

### Запуск локально

1. **Клонирование репозитория**
   ```bash
   git clone https://github.com/cutevil-magal/posmotri_v_okno.git
   cd posmotri_v_okno
   ```

2. **Запуск проекта**
   - Откройте файл `index.html` в браузере
   - Или используйте Live Server в VS Code

### Системные требования
- Современный браузер с поддержкой ES6+
- Доступ к интернету для работы с API
- Разрешение экрана не менее 320px

---

## 📁 Структура проекта

```
posmotri_v_okno/
├── index.html          # Главная страница
├── styles/
│   ├── style.css       # Основные стили
│   └── fonts/          # Локальные шрифты
├── scripts/            # JavaScript логика
├── images/             # Изображения и иконки
└── README.md           # Документация
```

---

## 🎨 Особенности реализации

### Семантическая разметка
```html
<main class="content">
  <section class="video-player">
    <video class="video-player__element" controls>
      <source src="video/sample.mp4" type="video/mp4">
    </video>
  </section>
  
  <section class="search">
    <form class="search__form">
      <input type="text" class="search__input" placeholder="Найти видео...">
    </form>
  </section>
</main>
```

### Адаптивная сетка карточек
```css
.video-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  padding: 20px;
}

.video-card {
  transition: transform 0.2s ease;
}

.video-card:hover {
  transform: translateY(-5px);
}
```

### Система состояний загрузки
```css
.loading::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 30px;
  height: 30px;
  border: 3px solid #f3f3f3;
  border-top: 3px solid #3498db;
  border-radius: 50%;
  animation: spin 1s linear infinite;
}

@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
```

---

## 🎯 Результаты реализации

**Достигнутые цели:**
- ✅ Полнофункциональный видео-плеер
- ✅ Адаптивная верстка для всех устройств
- ✅ Система поиска и фильтрации
- ✅ Оптимизация производительности
- ✅ Accessibility features (WCAG 2.1)

**Технические преимущества:**
- Чистая семантическая верстка
- Оптимизированные медиа-запросы
- Кастомные элементы интерфейса
- Плавные анимации CSS
- Кроссбраузерная совместимость

---

## 🔮 Планы по развитию

- [ ] PWA-функциональность (офлайн-режим)
- [ ] Кеширование запросов
- [ ] Расширенная аналитика пользовательского поведения
- [ ] Интеграция с социальными платформами
- [ ] Внедрение WebRTC для видеоконференций
- [ ] Система рекомендаций на основе ML

---

## 👩‍💻 Разработчик

**Анна Хвостикова** - Frontend Developer

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/cutevil-magal)
[![Email](https://img.shields.io/badge/Email-ana.magal@yandex.by-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ana.magal@yandex.by)

---

## 📄 Лицензия

Проект создан на основе дизайн-макета из Figma. Исходный код доступен для ознакомления и обучения.

**Макет в Figma:** [Ссылка на дизайн](https://www.figma.com/design/ApJjZAA3pBv2tCZM9E2ul2/2-%D1%81%D0%BF%D1%80%D0%B8%D0%BD%D1%82.-%D0%9F%D0%BE%D1%81%D0%BC%D0%BE%D1%82%D1%80%D0%B8-%D0%B2-%D0%BE%D0%BA%D0%BD%D0%BE?node-id=0-1&p=f&t=7qL4UTDYKuQaWvzj-0)

---
