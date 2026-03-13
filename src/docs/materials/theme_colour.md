---
title: 🎨 Тема и цвета
---
## Конфигурация темы

```yaml
theme:
  name: material
  language: ru
  palette:
    - scheme: default
      primary: deep purple
      accent: pink
      toggle:
        icon: material/weather-sunny
        name: Переключить на тёмную тему
    - scheme: slate
      primary: deep purple
      accent: pink
      toggle:
        icon: material/weather-night
        name: Переключить на светлую тему
```

---
## 🌈 Палитра цветов

| Параметр | Значение | Где применяется |
|--------|--------|----------|
| ``scheme: default`` | Светлая тема | 	Белый фон, тёмный текст |
| ``scheme: slate`` | Тёмная тема | 	Тёмно-серый фон, светлый текст |
| ``primary: deep purple`` | #673AB7 | 	Шапка, активные ссылки, заголовки |
| ``accent: pink`` | #E91E63 | 	Кнопки, ховеры, акценты |
| ``toggle.icon`` | 🌞 / | 	Переключатель темы в шапке |