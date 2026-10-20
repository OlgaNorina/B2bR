*This project has been created as part of the 42 curriculum by **onorina***
# Born2beRoot

## Description
This project focuses on setting up your first server as part of the School 42 curriculum.

## Defense Terminology & Comparisons

### 🖥️ Virtualization & Operating Systems (Виртуализация и ОС)

| Term / Comparison | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **VirtualBox** | A free tool (hypervisor) that lets you run another operating system (like Linux) inside your current computer. | Бесплатная программа (гипервизор), которая позволяет запускать одну ОС (например, Linux) внутри вашей текущей системы. |
| **UTM** | A lightweight tool similar to VirtualBox, but made specifically for Apple Silicon (M1/M2/M3) Mac computers. | Легковесный аналог VirtualBox, созданный специально для эффективной работы на компьютерах Mac с процессорами Apple Silicon (M-серия). |
| **Debian** | A very stable and reliable Linux operating system. It uses `.deb` packages and is famous for its strict open-source philosophy. | Очень стабильная и надежная ОС Linux. Использует пакеты `.deb` и известна своей строгой философией открытого ПО. |
| **Rocky Linux** | A stable, enterprise-grade Linux system. It was created to replace CentOS and is fully compatible with Red Hat Enterprise Linux (RHEL). | Стабильная корпоративная ОС Linux. Создана на замену CentOS и полностью совместима с Red Hat (RHEL). |
| **Debian vs Rocky Linux** | **Debian** is community-driven, uses `apt`, and values stability. **Rocky Linux** is enterprise-focused, uses `dnf`/`rpm`, and mimics commercial Red Hat systems. | **Debian** создается сообществом, использует `apt` и ценит стабильность. **Rocky Linux** ориентирован на бизнес, использует `dnf`/`rpm` и копирует коммерческую систему Red Hat. |
| **Red Hat (RHEL)** | Red Hat Enterprise Linux. A commercial, highly secure, and stable Linux operating system built for big businesses and servers. | Коммерческая, высокобезопасная и стабильная ОС Linux, созданная для крупного бизнеса и серверов. |
| **CentOS** | A free, community-supported Linux version that was identical to Red Hat. It was discontinued and replaced by newer systems like Rocky Linux. | Бесплатная версия Linux, которая была полной копией Red Hat. Проект закрыли, и его заменили новые системы, такие как Rocky Linux. |

### 🛡️ Security & Access Control (Безопасность и контроль доступа)

| Term / Comparison | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **SELinux** | A powerful Linux security system developed by the NSA. It controls exactly what processes and users can access on a very deep level. | Мощная система безопасности Linux, разработанная АНБ. Контролирует доступ процессов и пользователей на очень глубоком уровне. |
| **AppArmor** | A user-friendly security system for Linux. It protects the system by restricting what specific programs can do using easy-to-read profiles. | Простая система безопасности для Linux. Защищает систему, ограничивая действия конкретных программ с помощью понятных профилей. |
| **AppArmor vs SELinux** | **AppArmor** is easier to use and relies on path names to block programs. **SELinux** is much more secure but complex, using special security tags (labels) attached to files. | **AppArmor** проще и блокирует программы на основе путей к файлам. **SELinux** намного безопаснее, но сложнее, так как использует специальные метки безопасности для каждого файла. |
| **sudo** | "Superuser Do". A command that gives a regular user temporary administrator rights (root privileges) to run critical commands. | "Superuser Do" (выполнить суперпользователем). Команда, дающая обычному пользователю права администратора (root) для выполнения важных настроек. |

### 🔌 Network & Firewalls (Сеть и фаерволы)

| Term / Comparison | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **Port** | A virtual slot or door used by network protocols to identify which specific application or service should receive incoming data. | Виртуальная дверь (слот), используемая сетевыми протоколами, чтобы понять, какое именно приложение или служба должны получить входящие данные. |
| **Network traffic** | The data moving across a network at any given time, including files, website requests, and remote commands. | Данные, которые перемещаются по сети в любой момент времени, включая файлы, запросы к сайтам и удаленные команды. |
| **SSH** | Secure Shell. A secure, encrypted way to connect to and control your server from a remote computer. | Безопасный зашифрованный протокол для удаленного подключения к серверу и управления им с другого компьютера. |
| **Port 4242** | A custom communication port used in 42 school projects instead of the default SSH port (22) to practice server security configuration. | Кастомный порт, используемый в проектах 42 вместо стандартного SSH-порта (22) для практики настройки безопасности. |
| **UFW firewall** | Uncomplicated Firewall. A simple, easy-to-use tool to block or allow network traffic (default on Ubuntu/Debian). | Простой и понятный инструмент для блокировки или разрешения сетевого трафика (встроен по умолчанию в Ubuntu/Debian). |
| **firewalld** | A dynamic firewall tool used by default in Rocky/RHEL systems. It manages network traffic using "zones". | Динамический фаервол, используемый по умолчанию в системах Rocky/RHEL. Управляет трафиком с помощью разделения на "зоны". |
| **UFW vs firewalld** | **UFW** is simple, static, and perfect for basic setups. **firewalld** is more advanced, supports dynamic updates without restarting, and uses "zones". | **UFW** — простой, статический, идеален для базы. **firewalld** — продвинутый, поддерживает обновление правил без перезапуска и делит сеть на зоны. |

### 📦 Package Management (Управление пакетами)

| Term | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **apt** | The standard command-line tool in Debian to install, update, and remove software packages. | Стандартная консольная утилита в Debian для установки, обновления и удаления программ (пакетов). |
| **aptitude** | An advanced version of `apt` that includes a visual text interface and is much better at solving software conflicts. | Продвинутая версия `apt`, которая имеет псевдографический интерфейс и гораздо лучше решает конфликты зависимостей программ. |

### 💾 Storage Management (Управление дисками)

| Term | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **LVM** | Logical Volume Management. A tool that lets you group physical hard drives into flexible "virtual" partitions that can be easily resized. | Технология управления дисками. Позволяет объединять физические накопители в гибкие "виртуальные" разделы, размер которых можно легко менять на лету. |


