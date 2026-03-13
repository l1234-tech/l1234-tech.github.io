---
title: 📝 Markdown-расширения
---

## Полный список

```yaml
markdown_extensions:
  - attr_list
  - md_in_html
  - admonition
  - pymdownx.details
  - pymdownx.emoji:
      emoji_index: !!python/name:material.extensions.emoji.twemoji
      emoji_generator: !!python/name:material.extensions.emoji.to_svg
  - pymdownx.superfences
  - tables
  - toc:
      permalink: true
```

---

> ``attr_list`` — **Атрибуты элементов**

### Синтаксис:

```markdown
![Фото](photo.jpg){ width=300 align=right }
```

---

> ``admonition`` — **Блоки-подсказки**

### Синтаксис:

```markdown
!!! note "Заголовок"
    Текст примечания.
```

---

> ``pymdownx.details`` — **Сворачиваемые блоки**

### Синтаксис:

```markdown
??? example "Нажмите, чтобы раскрыть"
    Скрытый контент появится здесь.
```

---

> ``pymdownx.emoji`` — **Эмодзи**

### Синтаксис:

```markdown
pymdownx.emoji:
  emoji_index: !!python/name:material.extensions.emoji.twemoji
  emoji_generator: !!python/name:material.extensions.emoji.to_svg
```

### Использование:

```markdown
:material-school: — иконка Material  
:fontawesome-brands-github: — GitHub  
:smile: — эмодзи 😊
```

---

> ``pymdownx.superfences`` — Блоки кода

### Синтаксис:

```python
def foo():
    print("Hello, World!")
```

---

> ``tables`` — **Таблицы**

### Синтаксис:

```markdown
| Заголовок 1 | Заголовок 2 | Заголовок 3 |
|-------------|-------------|-------------|
| Ячейка 1    | Ячейка 2    | Ячейка 3    |
| Ячейка 4    | Ячейка 5    | Ячейка 6    |
```

---

> ``toc: permalink`` — **Ссылки на заголовки**

### Синтаксис:

```yaml
toc:
  permalink: true
```

---
