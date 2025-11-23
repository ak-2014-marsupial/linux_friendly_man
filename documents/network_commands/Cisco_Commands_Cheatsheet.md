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
| `interface range <діапазон>` | Одночасне налаштування діапазону (Fa0/1-10) або списку (Fa0/1, Gi0/1) портів. | `SW1(config)# interface range Fa0/1-10` |
| `ip address <ip-адреса> <маска>` | Призначення IP-адреси та маски підмережі. | `R1(config-if)# ip address 192.168.1.1 255.255.255.0` |
| `description <опис>` | Додавання опису для інтерфейсу (корисно для ідентифікації). | `R1(config-if)# description Link to LAN` |
| `shutdown` | Вимкнення інтерфейсу. | `R1(config-if)# shutdown` |
| `no shutdown` | Увімкнення інтерфейсу. | `R1(config-if)# no shutdown` |
| `ip default-gateway <ip-адреса>` | Встановлення шлюзу за замовчуванням (для комутаторів). | `SW1(config)# ip default-gateway 192.168.1.254` |

#### 3. Перевірка стану та конфігурації (`show` та інші команди)

Ці команди виконуються переважно у привілейованому режимі (`#`) і є ключовими для перевірки стану пристрою та правильності налаштувань.

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `show running-config` | Показати поточну (активну) конфігурацію. | `R1# show running-config` |
| `show startup-config` | Показати збережену конфігурацію, яка завантажиться при наступному старті. | `R1# show startup-config` |
| `show ip interface brief` | Показати короткий огляд стану всіх інтерфейсів, їх IP-адреси та статус ("up/up"). | `R1# show ip interface brief` |
| `show interfaces` | Показати детальну статистику та стан усіх інтерфейсів. | `R1# show interfaces` |
| `show ip route` | Показати таблицю маршрутизації. | `R1# show ip route` |
| `show version` | Показати версію IOS, час роботи пристрою та іншу системну інформацію. | `R1# show version` |
| `show mac address-table` | (На комутаторах) Показати таблицю MAC-адрес. | `SW1# show mac address-table` |
| `show vlan brief` | (На комутаторах) Показати інформацію про створені VLAN. | `SW1# show vlan brief` |
| `show interfaces trunk` | (На комутаторах) Показати стан транкових інтерфейсів та які VLAN через них передаються. | `SW1# show interfaces trunk` |
| `ping <ip-адреса>` | Перевірка мережевого з'єднання з іншим пристроєм (ICMP). | `R1# ping 192.168.1.2` |

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

#### 7. Управління VLAN (на комутаторах)

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `vlan <номер>` | Створює VLAN та переходить у режим його конфігурації. | `SW1(config)# vlan 10` |
| `name <ім'я_vlan>` | (в режимі `config-vlan`) Призначає ім'я для VLAN. | `SW1(config-vlan)# name Sales` |
| `switchport mode access` | (в режимі `config-if`) Переводить порт у режим доступу. | `SW1(config-if)# switchport mode access` |
| `switchport access vlan <номер>` | (в режимі `config-if`) Призначає порт доступу до вказаного VLAN. | `SW1(config-if)# switchport access vlan 10` |
| `switchport mode trunk` | (в режимі `config-if`) Переводить порт у режим магістралі (trunk). | `SW1(config-if)# switchport mode trunk` |
| `switchport trunk allowed vlan <список>` | (в режимі `config-if`) Вказує, які VLAN дозволено передавати через транк. | `SW1(config-if)# switchport trunk allowed vlan 10,20,99` |
| `no switchport mode trunk` | (в режимі `config-if`) Скасування режиму trunk для порту. | `SW1(config-if)# no switchport mode trunk` |

### 8. Приклади покрокового налаштування (Workflow)

Цей розділ демонструє повний цикл налаштування обладнання на двох типових прикладах, використовуючи рекомендовану 5-етапну послідовність.

#### Сценарій 1: Базове налаштування інтерфейсу роутера
**Завдання:** Налаштувати інтерфейс `GigabitEthernet0/0` роутера, призначити йому IP-адресу `192.168.1.1` та увімкнути його.

```cisco
// --- Крок 1: Вхід в режим конфігурації ---
Router> enable
Router# configure terminal
Router(config)# interface GigabitEthernet0/0

// --- Крок 2: Налаштування параметрів ---
Router(config-if)# description Management_Interface
Router(config-if)# ip address 192.168.1.1 255.255.255.0

// --- Крок 3: Активація інтерфейсу ---
Router(config-if)# no shutdown

// --- Крок 4: Перевірка (до збереження!) ---
Router(config-if)# end
Router# show ip interface brief
// * Переконайтесь, що статус інтерфейсу "up up"

Router# ping 192.168.1.1
// * Перевірте, що сам роутер відповідає на свою ж IP-адресу

// --- Крок 5: Збереження конфігурації ---
Router# copy running-config startup-config
// * Також можна використати стару, але досі популярну команду: write memory
```

#### Сценарій 2: Налаштування порту доступу (access port) на комутаторі
**Завдання:** Налаштувати порт `FastEthernet0/5` комутатора для підключення комп'ютера у `VLAN 20`.

```cisco
// --- Крок 1: Вхід в режим конфігурації ---
Switch> enable
Switch# configure terminal
// * Якщо VLAN ще не існує, його потрібно створити
Switch(config)# vlan 20
Switch(config-vlan)# name Staff_VLAN
Switch(config-vlan)# exit

Switch(config)# interface FastEthernet0/5

// --- Крок 2: Налаштування параметрів порту ---
Switch(config-if)# description User_PC_Port
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan 20

// --- Крок 3: Активація інтерфейсу ---
Switch(config-if)# no shutdown

// --- Крок 4: Перевірка (до збереження!) ---
Switch(config-if)# end
Switch# show vlan brief
// * Переконайтесь, що порт Fa0/5 з'явився у списку VLAN 20

Switch# show interfaces FastEthernet0/5 switchport
// * Перевірте, що "Administrative Mode" - static access, "Access Mode VLAN" - 20

// --- Крок 5: Збереження конфігурації ---
Switch# copy running-config startup-config
// * Також можна використати стару, але досі популярну команду: write memory
```

### 9. Налаштування та перевірка NAT
Команди для налаштування та моніторингу механізму трансляції мережевих адрес (Network Address Translation).

| Команда | Пояснення | Приклад |
| :--- | :--- | :--- |
| `ip nat inside` | (в режимі `config-if`) Позначає інтерфейс як внутрішній. | `R1(config-if)# ip nat inside` |
| `ip nat outside` | (в режимі `config-if`) Позначає інтерфейс як зовнішній. | `R1(config-if)# ip nat outside` |
| `access-list <номер> permit <source> <wildcard>` | Створює список доступу (ACL) для визначення трафіку, що підлягає NAT. | `R1(config)# access-list 1 permit 192.168.0.0 0.0.255.255` |
| `ip nat inside source list <ACL> interface <тип> <номер> overload` | Вмикає NAT Overload (PAT), транслюючи адреси з ACL в IP-адресу зовнішнього інтерфейсу. | `R1(config)# ip nat inside source list 1 interface Gi0/0 overload` |
| `show ip nat translations` | Показати поточну таблицю трансляцій NAT. | `Router# show ip nat translations` |
| `show ip nat statistics` | Відобразити статистику роботи NAT. | `Router# show ip nat statistics` |

---
#### Сценарій налаштування NAT Overload (PAT)
**Завдання:** Налаштувати роутер так, щоб усі комп'ютери з локальної мережі `192.168.1.0/24` могли виходити в Інтернет через єдину публічну IP-адресу, отриману на зовнішньому інтерфейсі `GigabitEthernet0/1`.

*   `GigabitEthernet0/0` - внутрішній інтерфейс (дивиться в локальну мережу).
*   `GigabitEthernet0/1` - зовнішній інтерфейс (дивиться в Інтернет).

```cisco
Router# configure terminal

// --- Крок 1: Визначення списку доступу (ACL) для внутрішніх адрес ---
// Дозволяємо всі адреси з мережі 192.168.1.0/24
Router(config)# access-list 1 permit 192.168.1.0 0.0.0.255

// --- Крок 2: Позначення інтерфейсів ---
// Внутрішній інтерфейс
Router(config)# interface GigabitEthernet0/0
Router(config-if)# ip nat inside
Router(config-if)# exit

// Зовнішній інтерфейс
Router(config)# interface GigabitEthernet0/1
Router(config-if)# ip nat outside
Router(config-if)# exit

// --- Крок 3: Створення правила NAT ---
// Вказуємо, що адреси зі списку ACL 1 потрібно транслювати
// в IP-адресу інтерфейсу Gi0/1 з перевантаженням (overload)
Router(config)# ip nat inside source list 1 interface GigabitEthernet0/1 overload

// --- Крок 4: Перевірка ---
Router(config)# end
Router# show ip nat translations
// * Після того, як внутрішній хост згенерує трафік в інтернет, тут з'являться записи
Router# show ip nat statistics
```
