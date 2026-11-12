# Совместный проект

Тестовый репозиторий для командной работы.

## Первый запуск

На macOS сначала установите Command Line Tools: `xcode-select --install`.
После установки проверьте: `git --version`.

```bash
git clone https://github.com/parallaxsizm/shdahsdgashgdasd.git
cd shdahsdgashgdasd
```

Откройте эту папку в VS Code. Для отправки изменений нужен доступ к репозиторию и вход в GitHub. Каждый участник использует свой аккаунт.

## Работа над задачей

1. Договоритесь, кто какую задачу делает и какие файлы меняет.
2. Перед новой задачей обновите main и создайте отдельную ветку:

```bash
git switch main
git pull --ff-only origin main
git switch -c feature/task-name
```

3. Измените файлы, проверьте результат и сохраните изменения в Git:

```bash
git status
git add path/to/changed-file
git commit -m "Describe the change"
git push -u origin feature/task-name
```

Замените `task-name`, путь и сообщение своими значениями. Для каждой задачи выбирайте новое имя ветки.

4. На GitHub создайте Pull request из своей ветки в main. Другой участник проверяет изменения; затем объедините их через Merge pull request.
5. После объединения вернитесь на main и выполните `git pull --ff-only origin main`.

## Договорённости

- main хранит общую рабочую версию; задачи делаем в отдельных ветках. Это договорённость команды, а не техническая блокировка.
- Не отправляем пароли, токены, API-ключи и файлы .env.
- Не используем force push в main.
- При конфликте вместе проверяем спорные строки и сохраняем нужные изменения обеих сторон.
- При первом коммите Git может попросить имя и email: настройте их локально через `git config user.name "Your Name"` и `git config user.email "YOUR_GITHUB_NOREPLY_EMAIL"`. Адрес noreply берите в GitHub Settings → Emails.

## Подключение команды

Владелец добавляет участников через Settings → Collaborators. Каждый принимает приглашение, клонирует репозиторий на свой компьютер и работает в своей ветке.

Стек проекта и команды запуска добавим после выбора задачи.
