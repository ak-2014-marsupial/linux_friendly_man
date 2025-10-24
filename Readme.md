*{{ site.annotation }}*

*{{ site.description }}*

[tldr (Too long; didn't read) - ще один ресурс с людським обличчям](https://tldr.sh/)

---

## 1. Теоретичні основи

- [Права доступу та спеціальні атрибути](./documents/concepts/permissions_and_special_attributes.md) — огляд стандартних та спеціальних прав доступу.
- [Ключові системні файли та директорії](./documents/concepts/key_files_and_directories.md) — огляд ключових файлів та директорій.
- [systemd](./documents/concepts/systemd.md) — огляд системи ініціалізації та менеджера сервісів.
- [Мережеві протоколи](./documents/concepts/network_protocols.md) — огляд протоколів моделі OSI.
- [Linux Network Troubleshooting](./documents/concepts/linux_network_troubleshooting.md) — посібник з діагностики мережевих проблем.
- [Курс "Linux и Администрирование" (на русском языке)](./documents/LinuxAndAdministration/Readme.md) — повний курс з адміністрування Linux.
- [Linux Obfuscation Techniques (на русском языке)](./documents/concepts/linux_obfuscation_techniques.md) — збірка трюків та технік для маскування активності в системі.
- [Кніги по Linux від linux-training.be (на англійскій)](https://linux-training.be/index.php?nav=home) - дуже якісний матеріал. 

### Performance troubleshooting

- [Діагностика продуктивності: CPU](./documents/concepts/Performance_troubleshooting/CPU%20Troubleshooting_uk.md) — аналіз та вирішення проблем з високим навантаженням на процесор.
- [Діагностика продуктивності: Memory](./documents/concepts/Performance_troubleshooting/Memory%20Troubleshooting_uk.md) — посібник з виявлення та усунення проблем з пам'яттю.
- [Діагностика продуктивності: HDD](./documents/concepts/Performance_troubleshooting/HDD_Troubleshooting_uk.md) — методи діагностики та вирішення проблем з продуктивністю жорсткого диска.
- [Методологія Аналізу Швидкодії Систем](./documents/concepts/Performance_troubleshooting/System_Performance_Analysis_Methodology_uk.md) — покроковий посібник з діагностики проблем продуктивності з використанням методів RED та USE.
- [Аналіз виводу vmstat: Поля та їх значення](./documents/process_and_system_monitoring/vmstat_fields.md) — детальний розбір полів команди vmstat та їх вплив на продуктивність.
- [Аналіз виводу iostat: Поля та їх значення](./documents/process_and_system_monitoring/iostat_fields.md) — детальний розбір полів команди iostat для діагностики продуктивності дисків.
- [Аналіз виводу top: Поля та їх значення](./documents/process_and_system_monitoring/top_fields.md) — детальний розбір полів команди top для моніторингу в реальному часі.
- [Аналіз виводу ss: Стани та черги сокетів](./documents/network_commands/ss_fields.md) — детальний розбір виводу команди ss для діагностики мережевих з'єднань.

## 2. Робота з файлами та директоріями

- [ls](./documents/file_and_directory_management/ls.md) (list) — вивести список файлів і директорій (читає метадані файлової системи).
- [cd](./documents/file_and_directory_management/cd.md) (change directory) — змінити поточну директорію.
- [pwd](./documents/file_and_directory_management/pwd.md) (print working directory) — показати повний шлях до поточної директорії ($PWD).
- [mkdir](./documents/file_and_directory_management/mkdir.md) (make directory) — створити нову директорію.
- [rmdir](./documents/file_and_directory_management/rmdir.md) (remove directory) — видалити порожню директорію.
- [touch](./documents/file_and_directory_management/touch.md) — створити порожній файл або змінити його час доступу/модифікації.
- [cp](./documents/file_and_directory_management/cp.md) (copy) — копіювати файли та директорії.
- [mv](./documents/file_and_directory_management/mv.md) (move) — перемістити або перейменувати файли та директорії.
- [rm](./documents/file_and_directory_management/rm.md) (remove) — видалити файли або директорії.
- [tree](./documents/file_and_directory_management/tree.md) (tree) — вивести структуру директорій у вигляді дерева.

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

- [find](./documents/file_and_text_search/find.md) — знайти файли та директорії за різними критеріями (читає метадані файлової системи).
- [locate](./documents/file_and_text_search/locate.md) — швидкий пошук файлів за індексованою базою даних (/var/lib/mlocate/mlocate.db).
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
- [su](./documents/user_and_permission_management/su.md) (switch user) — переключитися на іншого користувача (/etc/passwd, /etc/shadow).
- [sudo](./documents/user_and_permission_management/sudo.md) (superuser do) — виконати команду з правами адміністратора (/etc/sudoers).

## 6. Моніторинг та управління процесами

- [ps](./documents/process_and_system_monitoring/ps.md) (process status) — показати список поточних процесів (/proc/[pid]/stat, /proc/[pid]/status).
- [pstree](./documents/process_and_system_monitoring/pstree.md) (process status tree) — візуалізувати процеси у вигляді дерева (/proc/[pid]/stat).
- [top](./documents/process_and_system_monitoring/top.md) (table of processes) — динамічно відстежувати процеси та використання ресурсів (/proc/stat, /proc/meminfo, /proc/[pid]/stat).
- [htop](./documents/process_and_system_monitoring/htop.md) (Hisham's top) — покращена, інтерактивна версія top (/proc/stat, /proc/meminfo, /proc/[pid]/stat).
- [kill](./documents/process_and_system_monitoring/kill.md) — завершити процес за його ID (PID).
- [pkill](./documents/process_and_system_monitoring/pkill.md) (process kill) — завершити процес за його іменем.
- [pidstat](./documents/process_and_system_monitoring/pidstat.md) (process ID statistics) — моніторинг статистики для окремих процесів (/proc/[pid]/stat).
- [fuser](./documents/process_and_system_monitoring/fuser.md) (File USER) — ідентифікувати процеси, що використовують файли або сокети (/proc/[pid]/fd/).
- [lsof](./documents/process_and_system_monitoring/lsof.md) (list open files) — показати список файлів, відкритих процесами (/proc/[pid]/fd/).
- [strace](./documents/process_and_system_monitoring/strace.md) (system call trace) — трасування системних викликів і сигналів (syscall: ptrace).

## 7. Моніторинг системних ресурсів

- [df](./documents/process_and_system_monitoring/df.md) (disk free) — показати використання дискового простору (syscall: statfs).
- [du](./documents/process_and_system_monitoring/du.md) (disk usage) — оцінити розмір директорії або файлу (читає метадані файлової системи).
- [free](./documents/process_and_system_monitoring/free.md) — показати обсяг вільної та використаної пам'яті (/proc/meminfo).
- [iostat](./documents/process_and_system_monitoring/iostat.md) (input/output statistics) — моніторинг використання CPU та статистики вводу/виводу (/proc/diskstats, /proc/stat).
- [iotop](./documents/process_and_system_monitoring/iotop.md) (I/O top) — інтерактивний моніторинг дискового I/O по процесах (kernel I/O accounting interface).
- [mpstat](./documents/process_and_system_monitoring/mpstat.md) (multi-processor statistics) — моніторинг використання CPU по кожному ядру (/proc/stat).
- [sar](./documents/process_and_system_monitoring/sar.md) (system activity reporter) — зібрати, повідомити або зберегти інформацію про системну активність (/proc/, /var/log/sa/).
- [vmstat](./documents/process_and_system_monitoring/vmstat.md) (virtual memory statistics) — відстежувати віртуальну пам'ять, процеси та активність CPU (/proc/vmstat, /proc/stat).
- [cpustat](./documents/process_and_system_monitoring/cpustat.md) (CPU statistics) — моніторинг використання CPU окремими процесами (/proc/[pid]/stat).

## 8. Управління дисками та файловими системами

- [lsblk](./documents/disk_and_filesystem_management/lsblk.md) (list block devices) — вивести список блокових пристроїв (/sys/block).
- [fdisk](./documents/disk_and_filesystem_management/fdisk.md) (fixed disk) — маніпулювати таблицею розділів диска (таблиця розділів пристрою).
- [mkfs](./documents/disk_and_filesystem_management/mkfs.md) (make filesystem) — створити файлову систему Linux.
- [mount](./documents/disk_and_filesystem_management/mount.md) — змонтувати файлову систему (/proc/mounts).
- [blkid](./documents/disk_and_filesystem_management/blkid.md) (block ID) — знайти та роздрукувати атрибути блокових пристроїв (кеш /etc/blkid.tab, дані з пристроїв).

## 9. Управління пакетами

Для Debian/Ubuntu:
- [apt / apt-get](./documents/package_management/apt.md) (Advanced Package Tool) — керувати встановленням, оновленням та видаленням пакетів (/var/lib/dpkg/status, /var/lib/apt/lists/).

Для CentOS/Red Hat:
- yum / [dnf](./documents/package_management/dnf.md) (Dandified YUM) — керувати пакетами (/var/lib/rpm/Packages, /var/cache/dnf/).

- [dpkg](./documents/package_management/dpkg.md) (Debian package) — керувати пакетами в Debian-системах (/var/lib/dpkg/status).
- [rpm](./documents/package_management/rpm.md) (RPM Package Manager) — керувати пакетами в Red Hat-системах (/var/lib/rpm/Packages).

## 10. Робота з архівами

- [tar](./documents/archive_management/tar.md) (tape archive) — створити або розпакувати архіви (.tar, .tar.gz, .tar.bz2).
- [zip](./documents/archive_management/zip.md) та unzip — стиснути та розпакувати ZIP-архіви.
- [gzip](./documents/archive_management/gzip.md) (GNU zip) та gunzip — стиснути та розпакувати файли.
- [bzip2](./documents/archive_management/bzip2.md) — стиснення файлів з використанням алгоритму сортування блоків.

## 11. Мережеві команди

*Налаштування та моніторинг локальних інтерфейсів*
- [ip](./documents/network_commands/ip.md) — налаштування IP-адрес, інтерфейсів та маршрутизації (kernel netlink socket).
- [ethtool](./documents/network_commands/ethtool.md) (Ethernet tool) — перегляд та зміна параметрів мережевих карт (ioctl syscalls до драйвера).
- [netstat](./documents/network_commands/netstat.md) (network statistics) — аналіз активних з'єднань та відкритих портів (/proc/net/tcp).
- [ss](./documents/network_commands/ss.md) (socket statistics) — аналіз сокетів (kernel netlink socket).

*Робота з DNS*
- [host](./documents/network_commands/host.md) — проста утиліта для DNS-запитів (DNS-запити до сервера з /etc/resolv.conf).
- [nslookup](./documents/network_commands/nslookup.md) (name server lookup) — інтерактивна утиліта для запитів до DNS-серверів (DNS-запити до сервера з /etc/resolv.conf).
- [dig](./documents/network_commands/dig.md) (domain information groper) — інструмент для детальних DNS-запитів (DNS-запити до сервера з /etc/resolv.conf).

*Діагностика та сканування мережі*
- [ping](./documents/network_commands/ping.md) (Packet Inter-Network Groper) — перевірка доступності вузла та вимірювання затримки (мережеві пакети ICMP).
- [telnet](./documents/network_commands/telnet.md) (teletype network) — перевірка відкритості TCP-портів.
- [nc](./documents/network_commands/nc.md) (netcat) — утиліта для роботи з TCP/UDP, сканування, передачі даних.
- [traceroute](./documents/network_commands/traceroute.md) — відстеження маршруту пакетів до вузла (мережеві пакети UDP/ICMP).
- [nmap](./documents/network_commands/nmap.md) (network mapper) — сканер мереж для виявлення хостів та служб.
- [iftop](./documents/network_commands/iftop.md) (interface top) — інтерактивний моніторинг мережевого трафіку (захоплення пакетів з інтерфейсу).
- [nethogs](./documents/network_commands/nethogs.md) (network hogs) — моніторинг мережевого трафіку по процесах (/proc/net/tcp, /proc/[pid]/).

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

- [date](./documents/system_utilities/date.md) — показати або встановити системну дату та час (syscall: gettimeofday).
- [dmidecode](./documents/system_utilities/dmidecode.md) (DMI decode) — вивести інформацію про апаратне забезпечення (/dev/mem, /sys/firmware/dmi/tables/).
- [lshw](./documents/system_utilities/lshw.md) (list hardware) — вивести інформацію про апаратне забезпечення (/proc/, /sys/).
- [lspci](./documents/system_utilities/lspci.md) (list PCI) — вивести інформацію про PCI-пристрої (/sys/bus/pci).
- [lsusb](./documents/system_utilities/lsusb.md) (list USB) — вивести інформацію про USB-пристрої (/sys/bus/usb).

## 13. Системні утиліти

- [at](./documents/system_utilities/at.md) (at a specific time) — планувати одноразове виконання команд у вказаний час.
- [shutdown / reboot](./documents/system_utilities/shutdown.md) — вимкнути або перезавантажити систему.
- [history](./documents/system_utilities/history.md) — показати список раніше виконаних команд (~/.bash_history або аналог).
- [man](./documents/system_utilities/man.md) (manual) — відкрити довідкову сторінку для команди (/usr/share/man).
- [journalctl](./documents/system_utilities/journalctl.md) (journal control) — переглянути логи системи (у systemd) (/var/log/journal/).
- [systemctl](./documents/system_utilities/systemctl.md) (system control) — керування системними сервісами та станом системи (systemd).
- [crontab](./documents/system_utilities/crontab.md) (cron table) — планувати автоматичне виконання завдань (/var/spool/cron/).
- [screen](./documents/system_utilities/screen.md) (GNU Screen) — керування кількома термінальними сесіями (класичний аналог tmux).
- [tmux](./documents/system_utilities/tmux.md) (terminal multiplexer) — керування кількома термінальними сесіями в одному вікні.
- [Порівняння tmux та screen](./documents/system_utilities/ScreenVsTmux.md) — детальний аналіз та порівняння двох термінальних мультиплексорів.
- [tee](./documents/system_utilities/tee.md) (T-splitter) — читати зі стандартного вводу та записувати у стандартний вивід та файли.
- [type](./documents/system_utilities/type.md) — відобразити інформацію про тип команди (вбудована в оболонку).
- [xargs](./documents/system_utilities/xargs.md) (extended arguments) — побудувати та виконати командні рядки зі стандартного вводу.
