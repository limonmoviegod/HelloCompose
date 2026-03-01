▶Як запустити проєкт
Встановлення середовища
Встановити Android Studio (остання стабільна версія)
Встановити Android SDK (API 26+)
Створити емулятор через AVD Manager

Клонування репозиторію
git clone https://github.com/limonmoviegod/hellocompose.git
cd HelloCompose

Запуск
Відкрити проєкт у Android Studio
Дочекатися Gradle Sync
Натиснути Run ▶
Обрати емулятор або фізичний пристрій
GitFlow

У проєкті використовується стратегія GitFlow.
Основні гілки:
main — стабільна production-версія
develop — основна гілка розробки

git checkout develop
git checkout -b feature/new-feature
Структура проєкту
HelloCompose/
│
├── app/
│   ├── src/
│   ├── build.gradle.kts
│
├── .github/
│   ├── workflows/android-ci.yml
│   ├── ISSUE_TEMPLATE/
│
├── .gitignore
├── README.md
Issue Templates

Додано шаблони:
Bug Report
Feature Request
Pull Request Template

Розташування:
.github/ISSUE_TEMPLATE/
CI (Continuous Integration)

Налаштовано автоматичну перевірку через GitHub Actions.

CI виконує:
Збірку (assembleDebug)
Запуск unit-тестів
Lint перевірку

Workflow файл:
.github/workflows/android-ci.yml
CI запускається при:
push у main або develop
pull request у main або develop