*{{ site.annotation }}*

*{{ site.description }}*

---

## 1. Робота з файлами та директоріями

- [ls](./documents/file_and_directory_management/ls.md) (list) — вивести список файлів і директорій.
- [cd](./documents/file_and_directory_management/cd.md) (change directory) — змінити поточну директорію.
- [pwd](./documents/file_and_directory_management/pwd.md) (print working directory) — показати повний шлях до поточної директорії.
- [mkdir](./documents/file_and_directory_management/mkdir.md) (make directory) — створити нову директорію.
- [rmdir](./documents/file_and_directory_management/rmdir.md) (remove directory) — видалити порожню директорію.
- [touch](./documents/file_and_directory_management/touch.md) — створити порожній файл або змінити його час доступу/модифікації.
- [cp](./documents/file_and_directory_management/cp.md) (copy) — копіювати файли та директорії.
- [mv](./documents/file_and_directory_management/mv.md) (move) — перемістити або перейменувати файли та директорії.
- [rm](./documents/file_and_directory_management/rm.md) (remove) — видалити файли або директорії.

## 2. Перегляд та редагування файлів

- [cat](./documents/file_viewing_and_editing/cat.md) (concatenate) — вивести вміст файлу на екран.
- [less](./documents/file_viewing_and_editing/less.md) та [more](./documents/file_viewing_and_editing/more.md) — посторінково вивести вміст файлу.
- [head](./documents/file_viewing_and_editing/head.md) — показати перші рядки файлу.
- [tail](./documents/file_viewing_and_editing/tail.md) — показати останні рядки файлу.
- [nano](./documents/file_viewing_and_editing/nano.md) — простий текстовий редактор у терміналі.
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

- [useradd / adduser](./documents/user_and_permission_management/useradd.md) — створити нового користувача.
- [usermod](./documents/user_and_permission_management/usermod.md) — змінити параметри існуючого користувача.
- [userdel](./documents/user_and_permission_management/userdel.md) — видалити користувача.
- [groupadd](./documents/user_and_permission_management/groupadd.md) — створити нову групу.
- [passwd](./documents/user_and_permission_management/passwd.md) — змінити пароль користувача.
- [chmod](./documents/user_and_permission_management/chmod.md) (change mode) — змінити права доступу до файлів.
- [chown](./documents/user_and_permission_management/chown.md) (change owner) — змінити власника файлу/директорії.
- [chgrp](./documents/user_and_permission_management/chgrp.md) (change group) — змінити групу, до якої належить файл.
- [su](./documents/user_and_permission_management/su.md) (switch user) — переключитися на іншого користувача.
- [sudo](./documents/user_and_permission_management/sudo.md) (superuser do) — виконати команду з правами адміністратора.

## 5. Моніторинг процесів та системні ресурси

- [ps](./documents/process_and_system_monitoring/ps.md) (process status) — показати список поточних процесів.
- [top](./documents/process_and_system_monitoring/top.md) — динамічно відстежувати процеси та використання ресурсів.
- [htop](./documents/process_and_system_monitoring/htop.md) — покращена, інтерактивна версія top.
- [kill](./documents/process_and_system_monitoring/kill.md) — завершити процес за його ID (PID).
- [pkill](./documents/process_and_system_monitoring/pkill.md) — завершити процес за його іменем.
- [df](./documents/process_and_system_monitoring/df.md) (disk free) — показати використання дискового простору.
- [du](./documents/process_and_system_monitoring/du.md) (disk usage) — оцінити розмір директорії або файлу.
- [free](./documents/process_and_system_monitoring/free.md) — показати обсяг вільної та використаної пам'яті.

## 6. Управління пакетами

Для Debian/Ubuntu:
- [apt / apt-get](./documents/package_management/apt.md) — керувати встановленням, оновленням та видаленням пакетів.

Для CentOS/Red Hat:
- yum / [dnf](./documents/package_management/dnf.md) — керувати пакетами.

- [dpkg](./documents/package_management/dpkg.md) — керувати пакетами в Debian-системах.
- [rpm](./documents/package_management/rpm.md) — керувати пакетами в Red Hat-системах.

## 7. Робота з архівами

- [tar](./documents/archive_management/tar.md) — створити або розпакувати архіви (.tar, .tar.gz, .tar.bz2).
- [zip](./documents/archive_management/zip.md) та unzip — стиснути та розпакувати ZIP-архіви.
- [gzip](./documents/archive_management/gzip.md) та gunzip — стиснути та розпакувати файли.
- [bzip2](./documents/archive_management/bzip2.md) — стиснення файлів з використанням алгоритму сортування блоків.

## 8. Мережеві команди

*Налаштування та моніторинг локальних інтерфейсів*
- [ip](./documents/network_commands/ip.md) / ifconfig — показ та налаштування мережевих інтерфейсів.
- [netstat](./documents/network_commands/netstat.md) / ss — аналіз активних з'єднань та відкритих портів.

*Робота з DNS*
- [host](./documents/network_commands/host.md) — проста утиліта для DNS-запитів.
- [nslookup](./documents/network_commands/nslookup.md) — інтерактивна утиліта для запитів до DNS-серверів.
- [dig](./documents/network_commands/dig.md) — інструмент для детальних DNS-запитів.

*Діагностика та сканування мережі*
- [ping](./documents/network_commands/ping.md) — перевірка доступності вузла та вимірювання затримки.
- [telnet](./documents/network_commands/telnet.md) — перевірка відкритості TCP-портів.
- [nc](./documents/network_commands/nc.md) (netcat) — утиліта для роботи з TCP/UDP, сканування, передачі даних.
- [traceroute](./documents/network_commands/traceroute.md) — відстеження маршруту пакетів до вузла.
- [nmap](./documents/network_commands/nmap.md) — сканер мереж для виявлення хостів та служб.

*Передача даних та віддалене керування*
- [wget](./documents/network_commands/wget.md) / [curl](./documents/network_commands/curl.md) — завантаження файлів та даних з веб-ресурсів.
- [ssh](./documents/network_commands/ssh.md) — безпечне підключення до віддаленого сервера.
- [scp](./documents/network_commands/scp.md) — безпечне копіювання файлів між хостами.
- [rsync](./documents/network_commands/rsync.md) — ефективна синхронізація файлів та директорій.

*Безпека та шифрування*
- [openssl](./documents/network_commands/openssl.md) — набір інструментів для роботи з SSL/TLS та криптографією.
- [gpg](./documents/network_commands/gpg.md) — утиліта для шифрування та цифрового підпису (GNU Privacy Guard).
- [ssh-keygen](./documents/network_commands/ssh-keygen.md) — генерація ключів для SSH-аутентифікації.

## 9. Системні утиліти

- [shutdown / reboot](./documents/system_utilities/shutdown.md) — вимкнути або перезавантажити систему.
- [date](./documents/system_utilities/date.md) — показати або встановити системну дату та час.
- [history](./documents/system_utilities/history.md) — показати список раніше виконаних команд.
- [man](./documents/system_utilities/man.md) (manual) — відкрити довідкову сторінку для команди.
- [journalctl](./documents/system_utilities/journalctl.md) — переглянути логи системи (у systemd).
- [crontab](./documents/system_utilities/crontab.md) — планувати автоматичне виконання завдань.
- [type](./documents/system_utilities/type.md) — відобразити інформацію про тип команди.
- [xargs](./documents/system_utilities/xargs.md) — побудувати та виконати командні рядки зі стандартного вводу.

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
