#### Роботу виконав: Ігнатович Арсеній
# <h1 align="center"> СРС_WORK-CASE №1
#### Git — це найпопулярніша у світі розподілена система керування версіями, яку використовують для відстеження змін у файлах (найчастіше у вихідному коді програм) та спільної роботи над проєктами.
# 
## Для чого використовують Git?
- Збереження історії: Він фіксує кожен крок розробки. Якщо в коді з’явиться помилка, можна миттєво повернутися до будь-якої попередньої стабільної версії.
- Паралельна розробка: Завдяки системі гілок (branches) різні програмісти можуть одночасно працювати над різними функціями однієї програми, не заважаючи один одному.
- Командна співпраця: Git дозволяє об'єднувати код від багатьох розробників в один спільний проєкт і автоматично виявляє конфлікти, якщо двоє людей змінили один і той самий рядок.
- Надійність: Система є розподіленою, тобто повна копія всієї історії проєкту зберігається на комп'ютері кожного учасника команди.
## Основні поняття та дії в GitHub
- Репозиторії: Створення «папки» для проєкту. Вони бувають Public (бачать усі) та Private (доступні лише автору та запрошеним колегам).
- Форк: Копіювання чужого репозиторію до себе в профіль в один клік, щоб мати змогу редагувати його та експериментувати.
- Коміти в браузері: GitHub дозволяє створювати, редагувати файли та зберігати зміни (робити коміти) прямо в інтернеті без використання командного рядка.
- Запит на злиття: Інструмент, за допомогою якого один розробник просить автора проєкту перевірити та впровадити його код в основну версію.
- Issues (Проблеми/Завдання): Вбудований менеджер завдань, де користувачі можуть повідомляти про помилки в програмі, а автори — планувати нові функції.
## Команди на GitHub
- git clone (посилання на GitHub) — копіює проєкт із сайту GitHub на ваш комп'ютер.
- git pull — завантажує в комп'ютер найсвіжіші зміни, які ваші колеги завантажили на GitHub.
- git add  — готує всі ваші нові або змінені файли до збереження.
- git push origin main — найголовніша команда для GitHub. Вона відправляє ваші збережені коміти з комп'ютера прямо на сайт GitHub.
## Що таке коміт?
Коміт — це збережений «знімок» (або скріншот) стану ваших файлів у певний момент часу.
## Як коміт дозволяє відстежувати зміни?
- Зберігання дельти (різниці): Git порівнює поточний стан файлу з попереднім і записує лише те, що змінилося. Наприклад: «У файлі index.html додано 3 нові рядки та видалено 1». Це робить репозиторій дуже легким і швидким.
- Унікальний ідентифікатор: Кожному коміту присвоюється унікальний код із літер та цифр . Цей код гарантує, що історію неможливо непомітно підробити чи змінити — будь-яке втручання зламає цей шифр.
- Авторство та час: Кожен коміт чітко фіксує, хто саме зробив зміну (ім'я та email розробника) та коли це відбулося (дата й точний час).
- Коментарі (Commit Message): Створюючи коміт, розробник обов'язково пише пояснення (наприклад, git commit -m "Виправлено помилку в кнопці реєстрації"). Завдяки цьому інші люди  можуть відкрити історію і прочитати її як хронологічну книгу створення проєкту.
- Зв'язок у ланцюжок: Кожен новий коміт «знає», хто його «батько» (попередній коміт). Це створює безперервну історію, по якій можна переміщатися назад і вперед у часі.
## GitHub Glossary (Словник англійських термінів)
- Repository (Repo) — a digital storage location (folder) where all project files and their revision history are kept.
- Commit — a saved "snapshot" of the project's state at a specific point in time, identified by a unique ID and containing the author's notes.
- Branch — a parallel version of a repository, used to develop features or fix bugs in isolation without affecting the main code.
- Main / Master — the primary and stable branch of a repository that contains the production-ready code.
- Clone — a command used to create a local copy of a remote GitHub repository on a developer's computer.
- Push — the process of uploading local commits from a personal computer to the remote GitHub server.
- Pull — the process of downloading the latest changes from the GitHub server and merging them into the local files.
- Fork — a personal copy of another user's repository created in one's own profile to experiment with changes freely.
- Issue — a project management tool within GitHub used to report bugs, suggest new ideas, or track development tasks.
##  Conclusion
To sum up, GitHub is not just a place to store your code in the cloud. It is a super helpful tool for teamwork in programming. With GitHub, you can track all changes using commits, work on new features in different branches without breaking the main code, and easily share your work with classmates or colleagues. Today, every developer needs to know how to use Git and GitHub because it helps you move from small personal tasks to real team projects.
