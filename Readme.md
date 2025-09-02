*{{ site.annotation }}*

*{{ site.description }}*

---

## 1. Робота з файлами та директоріями

- [ls](./documents/file_and_directory_management/ls.md) (list) — вивести список файлів і директорій.
- cd (change directory) — змінити поточну директорію.
- pwd (print working directory) — показати повний шлях до поточної директорії.
- mkdir (make directory) — створити нову директорію.
- rmdir (remove directory) — видалити порожню директорію.
- touch — створити порожній файл або змінити його час доступу/модифікації.
- cp (copy) — копіювати файли та директорії.
- mv (move) — перемістити або перейменувати файли та директорії.
- rm (remove) — видалити файли або директорії.

## 2. Перегляд та редагування файлів

- cat (concatenate) — вивести вміст файлу на екран.
- [less](./documents/file_viewing_and_editing/less.md) та more — посторінково вивести вміст файлу.
- head — показати перші рядки файлу.
- tail — показати останні рядки файлу.
- nano — простий текстовий редактор у терміналі.
- [vi/vim](./documents/file_viewing_and_editing/vi.md) — потужний, але складніший текстовий редактор.
- [awk](./documents/file_viewing_and_editing/awk.md) — мова для сканування та обробки тексту.
- [sed](./documents/file_viewing_and_editing/sed.md) — потоковий редактор для фільтрації та перетворення тексту.
- [sort](./documents/file_viewing_and_editing/sort.md) — сортування рядків текстових файлів.
- [uniq](./documents/file_viewing_and_editing/uniq.md) — виведення або пропуск повторюваних рядків.

## 3. Пошук файлів та тексту

- [find](./documents/file_and_text_search/find.md) — знайти файли та директорії за різними критеріями.
- [locate](./documents/file_and_text_search/locate.md) — швидкий пошук файлів за індексованою базою даних.
- [grep](./documents/file_and_text_search/grep.md) (global regular expression print) — шукати текст всередині файлів.

## 4. Управління користувачами та правами доступу

- useradd / adduser — створити нового користувача.
- usermod — змінити параметри існуючого користувача.
- userdel — видалити користувача.
- groupadd — створити нову групу.
- passwd — змінити пароль користувача.
- chmod (change mode) — змінити права доступу до файлів.
- chown (change owner) — змінити власника файлу/директорії.
- chgrp (change group) — змінити групу, до якої належить файл.
- [su](./documents/user_and_permission_management/su.md) (switch user) — переключитися на іншого користувача.
- [sudo](./documents/user_and_permission_management/sudo.md) (superuser do) — виконати команду з правами адміністратора.

## 5. Моніторинг процесів та системні ресурси

- ps (process status) — показати список поточних процесів.
- [top](./documents/process_and_system_monitoring/top.md) — динамічно відстежувати процеси та використання ресурсів.
- htop — покращена, інтерактивна версія top.
- kill — завершити процес за його ID (PID).
- pkill — завершити процес за його іменем.
- [df](./documents/process_and_system_monitoring/df.md) (disk free) — показати використання дискового простору.
- [du](./documents/process_and_system_monitoring/du.md) (disk usage) — оцінити розмір директорії або файлу.
- [free](./documents/process_and_system_monitoring/free.md) — показати обсяг вільної та використаної пам'яті.

## 6. Управління пакетами

Для Debian/Ubuntu:
- apt / apt-get — керувати встановленням, оновленням та видаленням пакетів.

Для CentOS/Red Hat:
- yum / [dnf](./documents/package_management/dnf.md) — керувати пакетами.

- dpkg — керувати пакетами в Debian-системах.
- [rpm](./documents/package_management/rpm.md) — керувати пакетами в Red Hat-системах.

## 7. Робота з архівами

- [tar](./documents/archive_management/tar.md) — створити або розпакувати архіви (.tar, .tar.gz, .tar.bz2).
- [zip](./documents/archive_management/zip.md) та unzip — стиснути та розпакувати ZIP-архіви.
- [gzip](./documents/archive_management/gzip.md) та gunzip — стиснути та розпакувати файли.
- [bzip2](./documents/archive_management/bzip2.md) — стиснення файлів з використанням алгоритму сортування блоків.

## 8. Мережеві команди

- ping — перевірити доступність мережевого вузла.
- ssh (secure shell) — безпечно підключитися до віддаленого сервера.
- scp (secure copy) — безпечно копіювати файли між серверами.
- wget / curl — завантажити файли з інтернету.
- ifconfig / ip — показати інформацію про мережеві інтерфейси.
- netstat / ss — показати мережеві підключення та статистику.

## 9. Системні утиліти

- shutdown / reboot — вимкнути або перезавантажити систему.
- date — показати або встановити системну дату та час.
- history — показати список раніше виконаних команд.
- man (manual) — відкрити довідкову сторінку для команди.
- journalctl — переглянути логи системи (у systemd).
- crontab — планувати автоматичне виконання завдань.

## 10. Ключові системні файли та директорії

*Конфігураційні файли користувачів*
- **/etc/passwd**: Інформація про користувачів (без паролів).
- **/etc/shadow**: Хешовані паролі користувачів.
- **/etc/group**: Інформація про групи користувачів.
- **/etc/sudoers**: Налаштування доступу до команди sudo. Редагувати тільки через visudo!

*Системні конфігурації*
- **/etc/fstab**: Налаштування автоматичного монтування файлових систем.
- **/etc/hostname**: Ім'я хоста.
- **/etc/hosts**: Статичні відповідності IP-адрес та імен хостів.
- **/etc/resolv.conf**: IP-адреси DNS-серверів.
- **/etc/network/interfaces**: Налаштування мережевих інтерфейсів (для Debian/Ubuntu).
- **/etc/ssh/sshd_config**: Конфігураційний файл SSH-сервера.

*Журнали (логи)*
- **/var/log/**: Основна директорія для зберігання системних журналів.
- **/var/log/syslog** або **/var/log/messages**: Загальносистемні логи.
- **/var/log/auth.log** або **/var/log/secure**: Логи авторизації та безпеки.
- **/var/log/dmesg**: Повідомлення ядра системи.

*Інші важливі директорії*
- **/boot**: Файли для завантаження системи.
- **/home**: Домашні директорії користувачів.
- **/root**: Домашня директорія користувача root.
