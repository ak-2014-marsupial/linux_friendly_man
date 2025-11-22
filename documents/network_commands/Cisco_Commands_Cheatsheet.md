Звісно, я створю для вас довідник основних команд Cisco IOS, згрупорований за функціями, з поясненнями та прикладами.

### **Основи роботи в Cisco CLI**

Перш за все, важливо розуміти різні режими роботи командного рядка, оскільки доступні команди залежать від поточного режиму.

*   **User EXEC Mode (`>`):** Початковий режим. Дозволяє виконувати базові команди для моніторингу (`ping`, `show`).
*   **Privileged EXEC Mode (`#`):** Розширений режим. Дозволяє переглядати та змінювати конфігурацію. Перехід: `enable`.
*   **Global Configuration Mode (`(config)#`):** Режим для зміни глобальних налаштувань пристрою. Перехід: `configure terminal`.
*   **Interface Configuration Mode (`(config-if)#`):** Режим для налаштування конкретного мережевого інтерфейсу. Перехід: `interface <назва_інтерфейсу>`.
*   **Line Configuration Mode (`(config-line)#`):** Режим для налаштування ліній доступу (console, vty). Перехід: `line <тип_лінії> <номер>`.

---

### **Довідник команд Cisco IOS**

#### **1. Навігація та базові налаштування**

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `enable` | Перехід у привілейований режим. | `Router> enable` |
| `configure terminal` | Перехід у режим глобальної конфігурації. | `Router# configure terminal` |
| `exit` | Повернення до попереднього режиму. | `Router(config)# exit` |
| `end` | Повернення до привілейованого режиму з будь-якого підрежиму конфігурації. | `Router(config-if)# end` |
| `hostname <ім'я>` | Встановлення імені для пристрою. | `Router(config)# hostname R1` |
| `enable secret <пароль>` | Встановлення зашифрованого пароля для доступу до привілейованого режиму. | `R1(config)# enable secret class` |
| `banner motd #<повідомлення>#` | Встановлення банера "Message of the Day", який відображається при вході. | `R1(config)# banner motd #Welcome#`|
| `no <команда>` | Скасування або вимкнення раніше введеної команди. | `R1(config-if)# no shutdown` |

#### **2. Налаштування інтерфейсів**

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `interface <тип> <номер>` | Перехід до режиму конфігурації інтерфейсу. | `R1(config)# interface GigabitEthernet0/0` |
| `ip address <ip-адреса> <маска>` | Призначення IP-адреси та маски підмережі. | `R1(config-if)# ip address 192.168.1.1 255.255.255.0` |
| `description <опис>` | Додавання опису для інтерфейсу (корисно для ідентифікації). | `R1(config-if)# description Link to LAN` |
| `shutdown` | Вимкнення інтерфейсу. | `R1(config-if)# shutdown` |
| `no shutdown` | Увімкнення інтерфейсу. | `R1(config-if)# no shutdown` |
| `ip default-gateway <ip-адреса>` | Встановлення шлюзу за замовчуванням (для комутаторів). | `SW1(config)# ip default-gateway 192.168.1.254` |

#### **3. Перевірка стану та конфігурації (`show` команди)**

Ці команди виконуються переважно у привілейованому режимі (`#`).

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `show running-config` | Показати поточну (активну) конфігурацію. | `R1# show running-config` |
| `show startup-config` | Показати збережену конфігурацію, яка завантажиться при наступному старті. | `R1# show startup-config` |
| `show ip interface brief` | Показати короткий огляд стану всіх інтерфейсів, їх IP-адреси та статус. | `R1# show ip interface brief` |
| `show interfaces` | Показати детальну статистику та стан усіх інтерфейсів. | `R1# show interfaces` |
| `show ip route` | Показати таблицю маршрутизації. | `R1# show ip route` |
| `show version` | Показати версію IOS, час роботи пристрою та іншу системну інформацію. | `R1# show version` |
| `show mac address-table` | (На комутаторах) Показати таблицю MAC-адрес. | `SW1# show mac address-table` |
| `show vlan brief` | (На комутаторах) Показати інформацію про створені VLAN. | `SW1# show vlan brief` |

#### **4. Збереження та скидання конфігурації**

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `copy running-config startup-config` | Збереження поточної конфігурації в енергонезалежну пам'ять (NVRAM). | `R1# copy running-config startup-config` |
| `write memory` | Скорочений аналог попередньої команди. | `R1# write memory` |
| `erase startup-config` | Видалення збереженої конфігурації. | `R1# erase startup-config` |
| `reload` | Перезавантаження пристрою. | `R1# reload` |

#### **5. Налаштування безпеки доступу (лінії VTY та Console)**

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `line console 0` | Перехід до налаштування консольного доступу. | `R1(config)# line console 0` |
| `line vty 0 4` | Перехід до налаштування віддаленого доступу (Telnet/SSH) для 5 одночасних сесій. | `R1(config)# line vty 0 4` |
| `password <пароль>` | Встановлення пароля на лінію (для Telnet). | `R1(config-line)# password cisco` |
| `login` | Увімкнення перевірки пароля при вході на лінію. | `R1(config-line)# login` |
| `transport input ssh` | Дозволити підключення тільки через SSH (безпечніше, ніж Telnet). | `R1(config-line)# transport input ssh` |

#### **6. Налаштування маршрутизації**

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `ip route <мережа> <маска> <адреса_шлюзу>` | Створення статичного маршруту. | `R1(config)# ip route 10.0.0.0 255.0.0.0 192.168.1.2` |
| `router rip` | Увімкнення протоколу динамічної маршрутизації RIP. | `R1(config)# router rip` |
| `network <адреса_мережі>` | (В режимі `router`) Оголошення мережі, яка буде брати участь у динамічній маршрутизації. | `R1(config-router)# network 192.168.1.0` |

Сподіваюся, цей довідник буде корисним для вас.

#### 7. Управління VLAN (на комутаторах)

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `vlan <номер>` | Створює VLAN та переходить у режим його конфігурації. | `SW1(config)# vlan 10` |
| `name <ім'я_vlan>` | (в режимі `config-vlan`) Призначає ім'я для VLAN. | `SW1(config-vlan)# name Sales` |
| `switchport mode access` | (в режимі `config-if`) Переводить порт у режим доступу. | `SW1(config-if)# switchport mode access` |
| `switchport access vlan <номер>` | (в режимі `config-if`) Призначає порт доступу до вказаного VLAN. | `SW1(config-if)# switchport access vlan 10` |
| `switchport mode trunk` | (в режимі `config-if`) Переводить порт у режим магістралі (trunk). | `SW1(config-if)# switchport mode trunk` |
| `switchport trunk allowed vlan <список>` | (в режимі `config-if`) Вказує, які VLAN дозволено передавати через транк. | `SW1(config-if)# switchport trunk allowed vlan 10,20,99` |