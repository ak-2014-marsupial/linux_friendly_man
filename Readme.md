*{{ site.annotation }}*

*{{ site.description }}*

[tldr (Too long; didn't read) - ще один ресурс с людським обличчям](https://tldr.sh/)

---

## 1. Теоретичні основи

- [Права доступу та спеціальні атрибути](./documents/concepts/permissions_and_special_attributes.md) — огляд стандартних та спеціальних прав доступу.
- [Ключові системні файли та директорії](./documents/concepts/key_files_and_directories.md) — огляд ключових файлів та директорій.
- [Мережеві протоколи](./documents/concepts/network_protocols.md) — огляд протоколів моделі OSI.
- [Linux Network Troubleshooting](./documents/concepts/linux_network_troubleshooting.md) — посібник з діагностики мережевих проблем.
- [Курс "Linux и Администрирование" (на русском языке)](./documents/LinuxAndAdministration/Readme.md) — повний курс з адміністрування Linux.
- [Кніги по Linux від linux-training.be (на англійскій)](https://linux-training.be/index.php?nav=home) - дуже якісний матеріал. 

### Performance troubleshooting

- [Діагностика продуктивності: CPU](./documents/concepts/Performance_troubleshooting/CPU%20Troubleshooting_uk.md) — аналіз та вирішення проблем з високим навантаженням на процесор.
- [Діагностика продуктивності: Memory](./documents/concepts/Performance_troubleshooting/Memory%20Troubleshooting_uk.md) — посібник з виявлення та усунення проблем з пам'яттю.
- [Діагностика продуктивності: HDD](./documents/concepts/Performance_troubleshooting/HDD_Troubleshooting_uk.md) — методи діагностики та вирішення проблем з продуктивністю жорсткого диска.
- [Методологія Аналізу Швидкодії Систем](./documents/concepts/Performance_troubleshooting/System_Performance_Analysis_Methodology_uk.md) — покроковий посібник з діагностики проблем продуктивності з використанням методів RED та USE.

## 2. Робота з файлами та директоріями

- [ls](./documents/file_and_directory_management/ls.md) (list) — вивести список файлів і директорій.
- [cd](./documents/file_and_directory_management/cd.md) (change directory) — змінити поточну директорію.
- [pwd](./documents/file_and_directory_management/pwd.md) (print working directory) — показати повний шлях до поточної директорії.
- [mkdir](./documents/file_and_directory_management/mkdir.md) (make directory) — створити нову директорію.
- [rmdir](./documents/file_and_directory_management/rmdir.md) (remove directory) — видалити порожню директорію.
- [touch](./documents/file_and_directory_management/touch.md) — створити порожній файл або змінити його час доступу/модифікації.
- [cp](./documents/file_and_directory_management/cp.md) (copy) — копіювати файли та директорії.
- [mv](./documents/file_and_directory_management/mv.md) (move) — перемістити або перейменувати файли та директорії.
- [rm](./documents/file_and_directory_management/rm.md) (remove) — видалити файли або директорії.

## 3. Перегляд та редагування файлів

- [cat](./documents/file_viewing_and_editing/cat.md) (concatenate) — вивести вміст файлу на екран.
- [less](./documents/file_viewing_and_editing/less.md) та [more](./documents/file_viewing_and_editing/more.md) — посторінково вивести вміст файлу.
- [head](./documents/file_viewing_and_editing/head.md) — показати перші рядки файлу.
- [tail](./documents/file_viewing_and_editing/tail.md) — показати останні рядки файлу.
- [nano](./documents/file_viewing_and_editing/nano.md) (Nano's ANOther editor) — простий текстовий редактор у терміналі.
- [vi/vim](./documents/file_viewing_and_editing/vi.md) (visual / Vi IMproved) — потужний, але складніший текстовий редактор.
- [awk](./documents/file_viewing_and_editing/awk.md) (Aho, Weinberger, Kernighan) — мова для сканування та обробки тексту.
- [sed](./documents/file_viewing_and_editing/sed.md) (stream editor) — потоковий редактор для фільтрації та перетворення тексту.
- [sort](./documents/file_viewing_and_editing/sort.md) — сортування рядків текстових файлів.
- [uniq](./documents/file_viewing_and_editing/uniq.md) (unique) — виведення або пропуск повторюваних рядків.

## 4. Пошук файлів та тексту

- [find](./documents/file_and_text_search/find.md) — знайти файли та директорії за різними критеріями.
- [locate](./documents/file_and_text_search/locate.md) — швидкий пошук файлів за індексованою базою даних.
- [grep](./documents/file_and_text_search/grep.md) (global regular expression print) — шукати текст всередині файлів.

## 5. Управління користувачами та правами доступу

- [useradd / adduser](./documents/user_and_permission_management/useradd.md) — створити нового користувача.
- [usermod](./documents/user_and_permission_management/usermod.md) (user modify) — змінити параметри існуючого користувача.
- [userdel](./documents/user_and_permission_management/userdel.md) (user delete) — видалити користувача.
- [groupadd](./documents/user_and_permission_management/groupadd.md) — створити нову групу.
- [passwd](./documents/user_and_permission_management/passwd.md) (password) — змінити пароль користувача.
- [chmod](./documents/user_and_permission_management/chmod.md) (change mode) — змінити права доступу до файлів.
- [chown](./documents/user_and_permission_management/chown.md) (change owner) — змінити власника файлу/директорії.
- [chgrp](./documents/user_and_permission_management/chgrp.md) (change group) — змінити групу, до якої належить файл.
- [su](./documents/user_and_permission_management/su.md) (switch user) — переключитися на іншого користувача.
- [sudo](./documents/user_and_permission_management/sudo.md) (superuser do) — виконати команду з правами адміністратора.

## 6. Моніторинг та управління процесами

- [ps](./documents/process_and_system_monitoring/ps.md) (process status) — показати список поточних процесів.
- [pstree](./documents/process_and_system_monitoring/pstree.md) (process status tree) — візуалізувати процеси у вигляді дерева.
- [top](./documents/process_and_system_monitoring/top.md) (table of processes) — динамічно відстежувати процеси та використання ресурсів.
- [htop](./documents/process_and_system_monitoring/htop.md) (Hisham's top) — покращена, інтерактивна версія top.
- [kill](./documents/process_and_system_monitoring/kill.md) — завершити процес за його ID (PID).
- [pkill](./documents/process_and_system_monitoring/pkill.md) (process kill) — завершити процес за його іменем.
- [pidstat](./documents/process_and_system_monitoring/pidstat.md) (process ID statistics) — моніторинг статистики для окремих процесів.
- [fuser](./documents/process_and_system_monitoring/fuser.md) (File USER) — ідентифікувати процеси, що використовують файли або сокети.
- [lsof](./documents/process_and_system_monitoring/lsof.md) (list open files) — показати список файлів, відкритих процесами.
- [strace](./documents/process_and_system_monitoring/strace.md) (system call trace) — трасування системних викликів і сигналів.

## 7. Моніторинг системних ресурсів

- [df](./documents/process_and_system_monitoring/df.md) (disk free) — показати використання дискового простору.
- [du](./documents/process_and_system_monitoring/du.md) (disk usage) — оцінити розмір директорії або файлу.
- [free](./documents/process_and_system_monitoring/free.md) — показати обсяг вільної та використаної пам'яті.
- [iostat](./documents/process_and_system_monitoring/iostat.md) (input/output statistics) — моніторинг використання CPU та статистики вводу/виводу.
- [iotop](./documents/process_and_system_monitoring/iotop.md) (I/O top) — інтерактивний моніторинг дискового I/O по процесах.
- [mpstat](./documents/process_and_system_monitoring/mpstat.md) (multi-processor statistics) — моніторинг використання CPU по кожному ядру.
- [sar](./documents/process_and_system_monitoring/sar.md) (system activity reporter) — зібрати, повідомити або зберегти інформацію про системну активність.
- [vmstat](./documents/process_and_system_monitoring/vmstat.md) (virtual memory statistics) — відстежувати віртуальну пам'ять, процеси та активність CPU.
- [cpustat](./documents/process_and_system_monitoring/cpustat.md) (CPU statistics) — моніторинг використання CPU окремими процесами.

## 8. Управління дисками та файловими системами

- [lsblk](./documents/disk_and_filesystem_management/lsblk.md) (list block devices) — вивести список блокових пристроїв.
- [fdisk](./documents/disk_and_filesystem_management/fdisk.md) (fixed disk) — маніпулювати таблицею розділів диска.
- [mkfs](./documents/disk_and_filesystem_management/mkfs.md) (make filesystem) — створити файлову систему Linux.
- [mount](./documents/disk_and_filesystem_management/mount.md) — змонтувати файлову систему.
- [blkid](./documents/disk_and_filesystem_management/blkid.md) (block ID) — знайти та роздрукувати атрибути блокових пристроїв.

## 9. Управління пакетами

Для Debian/Ubuntu:
- [apt / apt-get](./documents/package_management/apt.md) (Advanced Package Tool) — керувати встановленням, оновленням та видаленням пакетів.

Для CentOS/Red Hat:
- yum / [dnf](./documents/package_management/dnf.md) (Dandified YUM) — керувати пакетами.

- [dpkg](./documents/package_management/dpkg.md) (Debian package) — керувати пакетами в Debian-системах.
- [rpm](./documents/package_management/rpm.md) (RPM Package Manager) — керувати пакетами в Red Hat-системах.

## 10. Робота з архівами

- [tar](./documents/archive_management/tar.md) (tape archive) — створити або розпакувати архіви (.tar, .tar.gz, .tar.bz2).
- [zip](./documents/archive_management/zip.md) та unzip — стиснути та розпакувати ZIP-архіви.
- [gzip](./documents/archive_management/gzip.md) (GNU zip) та gunzip — стиснути та розпакувати файли.
- [bzip2](./documents/archive_management/bzip2.md) — стиснення файлів з використанням алгоритму сортування блоків.

## 11. Мережеві команди

*Налаштування та моніторинг локальних інтерфейсів*
- [ip](./documents/network_commands/ip.md) — налаштування IP-адрес, інтерфейсів та маршрутизації (заміна `ifconfig`).
- [ethtool](./documents/network_commands/ethtool.md) (Ethernet tool) — перегляд та зміна параметрів мережевих карт.
- [netstat](./documents/network_commands/netstat.md) (network statistics) — аналіз активних з'єднань та відкритих портів (застаріла).
- [ss](./documents/network_commands/ss.md) (socket statistics) — аналіз сокетів (сучасна заміна для netstat).

*Робота з DNS*
- [host](./documents/network_commands/host.md) — проста утиліта для DNS-запитів.
- [nslookup](./documents/network_commands/nslookup.md) (name server lookup) — інтерактивна утиліта для запитів до DNS-серверів.
- [dig](./documents/network_commands/dig.md) (domain information groper) — інструмент для детальних DNS-запитів.

*Діагностика та сканування мережі*
- [ping](./documents/network_commands/ping.md) (Packet Inter-Network Groper) — перевірка доступності вузла та вимірювання затримки.
- [telnet](./documents/network_commands/telnet.md) (teletype network) — перевірка відкритості TCP-портів.
- [nc](./documents/network_commands/nc.md) (netcat) — утиліта для роботи з TCP/UDP, сканування, передачі даних.
- [traceroute](./documents/network_commands/traceroute.md) — відстеження маршруту пакетів до вузла.
- [nmap](./documents/network_commands/nmap.md) (network mapper) — сканер мереж для виявлення хостів та служб.
- [iftop](./documents/network_commands/iftop.md) (interface top) — інтерактивний моніторинг мережевого трафіку.
- [nethogs](./documents/network_commands/nethogs.md) (network hogs) — моніторинг мережевого трафіку по процесах.

*Передача даних та віддалене керування*
- [wget](./documents/network_commands/wget.md) (World Wide Web get) / [curl](./documents/network_commands/curl.md) (see URL) — завантаження файлів та даних з веб-ресурсів.
- [ssh](./documents/network_commands/ssh.md) (secure shell) — безпечне підключення до віддаленого сервера.
- [scp](./documents/network_commands/scp.md) (secure copy) — безпечне копіювання файлів між хостами.
- [rsync](./documents/network_commands/rsync.md) (remote sync) — ефективна синхронізація файлів та директорій.

*Безпека та шифрування*
- [openssl](./documents/network_commands/openssl.md) (Open Secure Sockets Layer) — набір інструментів для роботи з SSL/TLS та криптографією.
- [gpg](./documents/network_commands/gpg.md) (GNU Privacy Guard) — утиліта для шифрування та цифрового підпису.
- [ssh-keygen](./documents/network_commands/ssh-keygen.md) (secure shell key generation) — генерація ключів для SSH-аутентифікації.

## 12. Інформація про систему та обладнання

- [date](./documents/system_utilities/date.md) — показати або встановити системну дату та час.
- [dmidecode](./documents/system_utilities/dmidecode.md) (DMI decode) — вивести інформацію про апаратне забезпечення.
- [lshw](./documents/system_utilities/lshw.md) (list hardware) — вивести інформацію про апаратне забезпечення.
- [lspci](./documents/system_utilities/lspci.md) (list PCI) — вивести інформацію про PCI-пристрої.
- [lsusb](./documents/system_utilities/lsusb.md) (list USB) — вивести інформацію про USB-пристрої.

## 13. Системні утиліти

- [shutdown / reboot](./documents/system_utilities/shutdown.md) — вимкнути або перезавантажити систему.
- [history](./documents/system_utilities/history.md) — показати список раніше виконаних команд.
- [man](./documents/system_utilities/man.md) (manual) — відкрити довідкову сторінку для команди.
- [journalctl](./documents/system_utilities/journalctl.md) (journal control) — переглянути логи системи (у systemd).
- [crontab](./documents/system_utilities/crontab.md) (cron table) — планувати автоматичне виконання завдань.
- [tmux](./documents/system_utilities/tmux.md) (terminal multiplexer) — керування кількома термінальними сесіями в одному вікні.
- [type](./documents/system_utilities/type.md) — відобразити інформацію про тип команди.
- [xargs](./documents/system_utilities/xargs.md) (extended arguments) — побудувати та виконати командні рядки зі стандартного вводу.
