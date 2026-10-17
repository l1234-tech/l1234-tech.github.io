<div align="center">

# Андрей Сырчин · Portfolio

**Личное портфолио разработчика и учебный архив ИТМО**

[Открыть сайт](https://l1234-tech.github.io/) · [Проекты](https://l1234-tech.github.io/projects/) · [Обо мне](https://l1234-tech.github.io/about/) · [GitHub](https://github.com/l1234-tech)

![MkDocs](https://img.shields.io/badge/MkDocs-Material-7c3aed?style=flat-square&logo=materialformkdocs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222222?style=flat-square&logo=githubpages&logoColor=white)

</div>

---

## О репозитории

Этот репозиторий содержит исходный код моего **сайта-визитки и портфолио**, а также архив учебных работ. Сайт построен на **MkDocs Material** и публикуется на GitHub Pages через GitHub Actions.

Здесь можно найти информацию обо мне, проекты, участие в хакатонах, лабораторные работы и учебные материалы.

## Что есть внутри

| Раздел | Содержание |
|---|---|
| 🌐 [Сайт-портфолио](https://l1234-tech.github.io/) | Профиль, навыки, проекты, достижения и контакты |
| 🚀 Проекты | ML-сервис на FastAPI, перцептрон на C++, AI-ассистент и веб-проект по истории |
| 🏆 Хакатоны | Проектная школа «Авито» и «Цифровое здоровье» |
| 🧪 Лабораторные работы | Практические задания, исходный код, тесты и результаты |
| 📚 Материалы | Справка по MkDocs и учебные заметки |

## Структура репозитория

```text
.
├── .github/
│   └── workflows/
│       └── deploy.yaml       # Сборка и публикация сайта
├── src/
│   ├── mkdocs.yml            # Конфигурация MkDocs Material
│   └── docs/
│       ├── index.md          # Главная страница
│       ├── about.md          # Обо мне
│       ├── projects/         # Описание проектов
│       ├── hackathons/       # Хакатоны и проектные школы
│       ├── labs/             # Учебные лабораторные
│       ├── materials/        # Справочные материалы
│       └── assets/           # Изображения и пользовательские стили
├── 1_semestr/                # Учебные работы первого семестра
├── 2_semestr/                # Учебные работы второго семестра
├── requirements.txt          # Python-зависимости
└── README.md
```

## Технологии

- **MkDocs Material** — генерация документационного сайта и интерфейс.
- **Markdown** — содержимое страниц.
- **CSS** — дополнительные стили портфолио в `src/docs/assets/extra.css`.
- **Python** — окружение сборки и учебные проекты.
- **GitHub Actions + GitHub Pages** — автоматическая сборка и публикация.

## Запуск сайта локально

Требуется Python 3.11 или совместимая версия.

1. Склонируй репозиторий и перейди в него:

   ```bash
   git clone https://github.com/l1234-tech/l1234-tech.github.io.git
   cd l1234-tech.github.io
   ```

2. Создай виртуальное окружение:

   ```bash
   python -m venv .venv
   ```

   Активируй его:

   **Windows PowerShell**
   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

   **Linux / macOS**
   ```bash
   source .venv/bin/activate
   ```

3. Установи зависимости и запусти локальный сервер:

   ```bash
   python -m pip install -r requirements.txt
   cd src
   mkdocs serve -f mkdocs.yml -d ../site-preview
   ```

4. Открой адрес, который появится в терминале (обычно [http://127.0.0.1:8000](http://127.0.0.1:8000)).

Папка `site-preview/` — локальный результат сборки; её не нужно коммитить.

## Как публикуется сайт

Workflow [`.github/workflows/deploy.yaml`](.github/workflows/deploy.yaml) запускается при push в `main` и при pull request в эту ветку. Он устанавливает зависимости, проверяет наличие конфигурации, собирает сайт из `src/`, проверяет результат и публикует его на GitHub Pages.

**Чтобы изменить содержание сайта:**
1. Редактируй Markdown-файлы в `src/docs/`.
2. Для изменения внешнего вида редактируй `src/docs/assets/extra.css`.
3. Для изменения меню и параметров темы используй `src/mkdocs.yml`.
4. Отправь изменения в `main` — GitHub Actions выполнит сборку и публикацию.

Не редактируй сгенерированные HTML-файлы вместо исходных Markdown-страниц: при следующей сборке они будут созданы заново.

## Контакты

- **GitHub:** [@l1234-tech](https://github.com/l1234-tech)
- **Telegram:** [@dark_kurom1](https://t.me/dark_kurom1)
- **Email:** [syrchin.andrej@inbox.ru](mailto:syrchin.andrej@inbox.ru)

---

<div align="center">

*Сделано Андреем Сырчиным · 2026*

</div>
