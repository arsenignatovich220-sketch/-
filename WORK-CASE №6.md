#### Роботу виконав: Ігнатович Арсеній
# <h1 align="center"> СРС_WORK-CASE №6
### Словник термінів:
- Command-Line Interpreter (Shell) — командний інтерпретатор (оболонка), програма-посередник, яка приймає текстові команди від користувача, перекладає їх мовою операційної системи та виводить результат виконання на екран.
- Bash (Bourne Again Shell) — стандартний командний інтерпретатор у більшості дистрибутивів Linux, який використовується для виконання команд та написання системних скриптів.
- Zsh (Z Shell) — розширений командний інтерпретатор, сумісний із Bash, що має покращене автодоповнення, виправлення друкарських помилок та підтримку плагінів.
- Fish (Friendly Interactive Shell) — інтерактивна командна оболонка, орієнтована на зручність роботи завдяки підсвічуванню синтаксису в реальному часі та розумним автопідказкам без складного налаштування.
- Package Manager — менеджер пакетів (наприклад, apt, dnf, pacman), системна утиліта для автоматичного встановлення, оновлення та видалення програмного забезпечення з офіційних репозиторіїв.
- User Account — обліковий запис користувача, набір даних у системі, який ідентифікує конкретну особу чи службу та визначає її права доступу, домашній каталог і оболонку за замовчуванням.
- User Group — група користувачів, логічне об'єднання кількох облікових записів для зручного керування спільними правами доступу до файлів, каталогів та системних ресурсів.
- Root (Superuser) — суперкористувач, головний адміністративний обліковий запис у Linux із необмеженими правами на зміну будь-яких налаштувань та файлів операційної системи.
- Sudo (Superuser Do) — утиліта, яка дозволяє звичайному авторизованому користувачеві тимчасово виконувати окремі команди з правами суперкористувача (root).
- Home Directory — домашній каталог (/home/ім'я_користувача), особиста папка користувача в системі, де зберігаються його власні файли та персональні налаштування програм.
- Nologin (/usr/sbin/nologin) — спеціальна фіктивна оболонка-заглушка, яка призначається обліковим записам для заборони інтерактивного входу в систему через термінал або SSH.
- Environment Variables — змінні середовища (наприклад, $SHELL, $PATH, $USER), динамічні параметри операційної системи, які зберігають інформацію про поточну сесію та налаштування робочого простору.
- Working Directory — поточний робочий каталог, директорія файлової системи, у якій користувач перебуває в конкретний момент роботи в терміналі (перевіряється командою pwd).
- System Configuration — системна конфігурація, сукупність апаратних і програмних параметрів операційної системи, таких як версія ядра, ім'я хоста, обсяг пам'яті та дискового простору.
### 1.Встановлення декількох командних інтерпретаторів:
#### 1)Команди для встановлення:
- Оновлення списку пакетів:
  - sudo apt update
- Встановлення Zsh (Z Shell):
  - sudo apt install zsh -y
- Встановлення Fish (Friendly Interactive Shell):
  - sudo apt install fish -y
#### 2) Короткий опис можливостей:
##### Zsh (Z Shell)
Zsh — це розширена версія стандартної оболонки Bourne Shell, яка повністю сумісна зі скриптами Bash, але пропонує значно більше функцій для інтерактивної роботи.
- Розумне автодоповнення: Підтримує контекстне доповнення не лише шляхів до файлів, а й аргументів команд, прапорців, гілок Git та змінних середовища.
- Виправлення помилок: Автоматично пропонує виправити друкарські помилки у введених командах чи шляхах.
- Спільна історія команд: Дозволяє ділитися історією виконаних команд між кількома одночасно відкритими вкладками або вікнами термінала.
- Екосистема плагінів і тем: Має величезну кількість фреймворків (наприклад, Oh My Zsh), які дозволяють легко налаштовувати зовнішній вигляд рядка запиту та додавати нові функції.
##### Fish (Friendly Interactive Shell)
Fish — це сучасний командний інтерпретатор, створений з акцентом на зручність використання «з коробки» без необхідності складного попереднього налаштування.
- Підсвічування синтаксису в реальному часі: Під час введення команди правильні команди та існуючі шляхи підсвічуються одним кольором, а неіснуючі або помилкові — червоним.
- Автопідказки (Autosuggestions): Аналізує історію команд і поточну директорію, пропонуючи сірим текстом продовження команди прямо під час набору (приймається клавішею →).
- Веб-інтерфейс для налаштувань: Дозволяє змінювати кольорові схеми та налаштовувати рядок запиту через зручну сторінку у браузері за допомогою команди fish_config.
- Зрозуміліший синтаксис скриптів: Відмовляється від застарілих конструкцій POSIX на користь більш читабельного та логічного синтаксису для написання власних функцій.
### 2.Створення 10 нових користувачів в моїй системі:
#### 1) Створення груп:
- sudo groupadd technical_support
- sudo groupadd developers
- sudo groupadd financiers
- sudo groupadd founders
- sudo groupadd guests
#### 2)Створення користувачів та додавання їх до груп:
- Група Technical support (2 користувачі):
  - sudo useradd -m -s /bin/bash -G technical_support admin_ivan
  - sudo useradd -m -s /bin/bash -G technical_support sys_olena
- Група Developers (3 користувачі):
  - sudo useradd -m -s /bin/bash -G developers dev_andriy
  - sudo useradd -m -s /bin/bash -G developers dev_maria
  - sudo useradd -m -s /bin/bash -G developers dev_taras
- Група Financiers (2 користувачі):
  - sudo useradd -m -s /bin/bash -G financiers fin_iryna
  - sudo useradd -m -s /bin/bash -G financiers fin_dmytro
- Група Founders (2 користувачі):
  - sudo useradd -m -s /bin/bash -G founders ceo_oleksandr
  - sudo useradd -m -s /bin/bash -G founders cto_nataliya
- Група Guests (1 користувач):
  - sudo useradd -m -s /bin/bash -G guests guest_user
### 3.Командні інтерпретатори для кожного з користувачів:
- Technical support — оболонка bash:
  - sudo usermod -s /bin/bash admin_ivan
  - sudo usermod -s /bin/bash sys_olena
- Developers — інтерпретатор 1 (zsh):
  - sudo usermod -s /usr/bin/zsh dev_andriy
  - sudo usermod -s /usr/bin/zsh dev_maria
  - sudo usermod -s /usr/bin/zsh dev_taras
- Financiers — заборона доступу до оболонок (nologin):
  - sudo usermod -s /usr/sbin/nologin fin_iryna
  - sudo usermod -s /usr/sbin/nologin fin_dmytro
- Founders — інтерпретатор 2 (fish):
  - sudo usermod -s /usr/bin/fish ceo_oleksandr
  - sudo usermod -s /usr/bin/fish cto_nataliya
- Guests — заборона доступу до оболонок (nologin):
  - sudo usermod -s /usr/sbin/nologin guest_user
### 4.Демонстрація прикладів роботи:
| Група | Користувач | Оболонка | Ключова команда перевірки | Результат роботи |
| :--- | :--- | :--- | :--- | :--- |
| Technical support | admin_ivan | /bin/bash | uname -a, df -h | Успішний вхід, вивід даних про ядро та диски |
| Developers	| dev_andriy | /usr/bin/zsh | pwd, echo $ZSH_VERSION | Успішний вхід у Zsh, вивід поточного каталогу |
| Founders | ceo_oleksandr | /usr/bin/fish | date, uptime | Успішний вхід у Fish, вивід системної дати |
| Financiers | fin_iryna | /usr/sbin/nologin | su - fin_iryna | Відмова у доступі (Account not available) |
| Guests | guest_user | /usr/sbin/nologin | su - guest_user | Відмова у доступі (Account not available) |
### Висновок:
During this practical work, I learned how to install and configure different command-line interpreters in the Linux operating system. In addition to the standard Bash shell, I installed Zsh and Fish using the system package manager and explored their main features, such as auto-completion and syntax highlighting.
I also practiced basic user administration by creating ten new user accounts and organizing them into five functional groups: Technical support, Developers, Financiers, Founders, and Guests. For each group, I configured a specific default shell using the usermod utility. In particular, I restricted terminal access for the Financiers and Guests groups by assigning them the /usr/sbin/nologin shell to improve system security. Finally, I tested the accounts by logging in and running basic commands to check system information, current directories, and the system date. This work helped me understand how user permissions and command shells are managed in a multi-user environment.

