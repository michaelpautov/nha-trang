# Onboarding: Начало работы с проектом

Пошаговая инструкция для нового разработчика.

---

## 1. Получи доступ к аккаунту

1. Открой почту, которую тебе дали
2. Проверь входящие — там может быть письмо для подтверждения

---

## 2. Установи Claude Code

### macOS

```bash
# Через npm (нужен Node.js 18+)
npm install -g @anthropic-ai/claude-code

# Или через Homebrew
brew install claude-code
```

### Проверь установку

```bash
claude --version
```

Если команда не найдена — установи Node.js:
```bash
# Через Homebrew
brew install node

# Или скачай с https://nodejs.org/
```

---

## 3. Авторизуйся в Claude Code

```bash
claude
```

При первом запуске:
1. Откроется браузер для авторизации
2. Войди через почту, которую тебе дали
3. Подтверди доступ
4. Вернись в терминал — должно написать что авторизация успешна

---

## 4. Склонируй репозиторий

```bash
# Перейди в папку для проектов
cd ~/Projects

# Склонируй репозиторий
git clone https://github.com/michaelpautov/nha-trang.git

# Перейди в папку проекта
cd nha-trang
```

---

## 5. Запусти Claude Code в проекте

```bash
claude
```

Claude автоматически прочитает `CLAUDE.md` и поймёт контекст проекта.

---

## 6. Если чего-то не хватает

### Git не установлен

```bash
# macOS
brew install git

# Или скачай с https://git-scm.com/
```

### Node.js не установлен

```bash
# macOS
brew install node

# Или скачай с https://nodejs.org/ (LTS версия)
```

### npm выдаёт ошибки прав доступа

```bash
# Исправить права
sudo chown -R $(whoami) ~/.npm
```

### Homebrew не установлен (macOS)

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

## 7. Начни работу

После запуска `claude` в папке проекта, можешь сказать:

> "Прочитай документацию в docs/ и расскажи что нужно делать дальше"

Или:

> "Какие user stories ещё не реализованы?"

---

## Структура проекта

```
nha-trang/
├── CLAUDE.md           # Контекст для AI (читает автоматически)
├── README.md           # Описание проекта
├── ONBOARDING.md       # Эта инструкция
└── docs/
    ├── user-stories.md # User stories
    ├── data-models.md  # Схема базы данных
    └── pages.md        # Макеты страниц
```

---

## Контакты

Если что-то не работает — пиши в Telegram: [указать контакт]

---

Удачи!
