*This project has been created as part of the 42 curriculum by **onorina***
# Born2beRoot

## Description
This project focuses on setting up the first server as part of the School 42 curriculum.

### Defense Terminology & Comparisons

#### 🖥️ Virtualization & Operating Systems (Виртуализация и ОС)
<details>
  
| Term / Comparison | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **VirtualBox** | A free tool (hypervisor) that lets you run another operating system (like Linux) inside your current computer. | Бесплатная программа (гипервизор), которая позволяет запускать одну ОС (например, Linux) внутри вашей текущей системы. |
| **UTM** | A lightweight tool similar to VirtualBox, but made specifically for Apple Silicon (M1/M2/M3) Mac computers. | Легковесный аналог VirtualBox, созданный специально для эффективной работы на компьютерах Mac с процессорами Apple Silicon (M-серия). |
| **Debian** | A very stable and reliable Linux operating system. It uses `.deb` packages and is famous for its strict open-source philosophy. | Очень стабильная и надежная ОС Linux. Использует пакеты `.deb` и известна своей строгой философией открытого ПО. |
| **Rocky Linux** | A stable, enterprise-grade Linux system. It was created to replace CentOS and is fully compatible with Red Hat Enterprise Linux (RHEL). | Стабильная корпоративная ОС Linux. Создана на замену CentOS и полностью совместима с Red Hat (RHEL). |
| **Debian vs Rocky Linux** | **Debian** is community-driven, uses `apt`, and values stability. **Rocky Linux** is enterprise-focused, uses `dnf`/`rpm`, and mimics commercial Red Hat systems. | **Debian** создается сообществом, использует `apt` и ценит стабильность. **Rocky Linux** ориентирован на бизнес, использует `dnf`/`rpm` и копирует коммерческую систему Red Hat. |
| **Red Hat (RHEL)** | Red Hat Enterprise Linux. A commercial, highly secure, and stable Linux operating system built for big businesses and servers. | Коммерческая, высокобезопасная и стабильная ОС Linux, созданная для крупного бизнеса и серверов. |
| **CentOS** | A free, community-supported Linux version that was identical to Red Hat. It was discontinued and replaced by newer systems like Rocky Linux. | Бесплатная версия Linux, которая была полной копией Red Hat. Проект закрыли, и его заменили новые системы, такие как Rocky Linux. |
  
</details>

#### 🛡️ Security & Access Control (Безопасность и контроль доступа)
<details>

| Term / Comparison | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **SELinux** | A powerful Linux security system developed by the NSA. It controls exactly what processes and users can access on a very deep level. | Мощная система безопасности Linux, разработанная АНБ. Контролирует доступ процессов и пользователей на очень глубоком уровне. |
| **AppArmor** | A user-friendly security system for Linux. It protects the system by restricting what specific programs can do using easy-to-read profiles. | Простая система безопасности для Linux. Защищает систему, ограничивая действия конкретных программ с помощью понятных профилей. |
| **AppArmor vs SELinux** | **AppArmor** is easier to use and relies on path names to block programs. **SELinux** is much more secure but complex, using special security tags (labels) attached to files. | **AppArmor** проще и блокирует программы на основе путей к файлам. **SELinux** намного безопаснее, но сложнее, так как использует специальные метки безопасности для каждого файла. |
| **sudo** | "Superuser Do". A command that gives a regular user temporary administrator rights (root privileges) to run critical commands. | "Superuser Do" (выполнить суперпользователем). Команда, дающая обычному пользователю права администратора (root) для выполнения важных настроек. |

</details>

#### 🔌 Network & Firewalls (Сеть и фаерволы)
<details>

| Term / Comparison | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **Port** | A virtual slot or door used by network protocols to identify which specific application or service should receive incoming data. | Виртуальная дверь (слот), используемая сетевыми протоколами, чтобы понять, какое именно приложение или служба должны получить входящие данные. |
| **Network traffic** | The data moving across a network at any given time, including files, website requests, and remote commands. | Данные, которые перемещаются по сети в любой момент времени, включая файлы, запросы к сайтам и удаленные команды. |
| **SSH** | Secure Shell. A secure, encrypted way to connect to and control your server from a remote computer. | Безопасный зашифрованный протокол для удаленного подключения к серверу и управления им с другого компьютера. |
| **Port 4242** | A custom communication port used in 42 school projects instead of the default SSH port (22) to practice server security configuration. | Кастомный порт, используемый в проектах 42 вместо стандартного SSH-порта (22) для практики настройки безопасности. |
| **UFW firewall** | Uncomplicated Firewall. A simple, easy-to-use tool to block or allow network traffic (default on Ubuntu/Debian). | Простой и понятный инструмент для блокировки или разрешения сетевого трафика (встроен по умолчанию в Ubuntu/Debian). |
| **firewalld** | A dynamic firewall tool used by default in Rocky/RHEL systems. It manages network traffic using "zones". | Динамический фаервол, используемый по умолчанию в системах Rocky/RHEL. Управляет трафиком с помощью разделения на "зоны". |
| **UFW vs firewalld** | **UFW** is simple, static, and perfect for basic setups. **firewalld** is more advanced, supports dynamic updates without restarting, and uses "zones". | **UFW** — простой, статический, идеален для базы. **firewalld** — продвинутый, поддерживает обновление правил без перезапуска и делит сеть на зоны. |

</details>

#### 📦 Package Management (Управление пакетами)
<details>

| Term | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **apt** | The standard command-line tool in Debian to install, update, and remove software packages. | Стандартная консольная утилита в Debian для установки, обновления и удаления программ (пакетов). |
| **aptitude** | An advanced version of `apt` that includes a visual text interface and is much better at solving software conflicts. | Продвинутая версия `apt`, которая имеет псевдографический интерфейс и гораздо лучше решает конфликты зависимостей программ. |

</details>

#### 💾 Storage Management (Управление дисками)
<details>

| Term | Simple English Definition | Описание на русском |
| :--- | :--- | :--- |
| **LVM** | Logical Volume Management. A tool that lets you group physical hard drives into flexible "virtual" partitions that can be easily resized. | Технология управления дисками. Позволяет объединять физические накопители в гибкие "виртуальные" разделы, размер которых можно легко менять на лету. |

</details>


## Instructions

### 📚 Structure
1. 🛠️ **Virtual Machine Setup** - Installing VirtualBox and setting up your VM
1. 🌀 **Debian Installation** - Complete OS installation with proper partitioning
1. ⚙️ **System Configuration** - SSH, firewall, users, and security policies
1. 🧾 **Monitoring** - Creating and scheduling monitoring scripts
1. ✅ **Evaluation Preparation** - Commands and answers for peer evaluation

### Step 1 📥 Prerequisites

The following software was pre-installed and configured on the host machine to develop this project:

* **Virtualization Software (Choose one based on your OS):**
  * [Download VirtualBox](https://virtualbox.org) — Recommended for Windows, Linux, and Intel-based Macs.
* **Operating System Image:**
  * [Download Debian 12.5.0 Netinst ISO (amd64)](https://debian.org) — The lightweight, official installer used to set up the server from scratch.

### Stp 2 💻 Creating the Virtual Machine
 
#### Recommended VM Hardware Allocation

When creating the Virtual Machine in VirtualBox / UTM, use the following resource allocation:

* **RAM (ОЗУ):** **1024 MB (1 GB)** — Plenty for a headless Linux server running background scripts. (Do not allocate more than 2048 MB unless doing heavy tasks).
* **CPU (Процессор):** **1 vCPU** — A single virtual core is more than enough for system administration tasks and light services.
* **Storage (Диск):** **8.5 GB** (VDI / Dynamic Allocation) — Plenty of space to easily fit the required encrypted LVM partition scheme for the mandatory part without wasting host storage.
  * 💾 **Mandatory LVM Partition Scheme (8.5 GB Disk)**
    <details>
    The drive is partitioned strictly according to the mandatory requirements using Encrypted LVM:
    
    * **/boot** — **≈500 MB** *(Standard Partition / Non-Encrypted)*
      * Stores the Linux kernel and bootloader files. It must remain unencrypted so the system can boot and ask for the decryption password.
      * *Хранит ядро Linux и файлы загрузчика. Остается незашифрованным, чтобы система могла запуститься и запросить пароль.*
    * **/root** — **≈3 GB** *(Logical Volume / Encrypted)*
      * The main system partition. It automatically includes directories like `/var` (and `/var/log/sudo/`), `/tmp`, sharing this volume's total capacity.
      * *Главный системный раздел. Автоматически включает в себя папки `/var` (включая логи sudo), `/tmp`, которые делят между собой это пространство.*
    * **/home** — **≈4 GB** *(Logical Volume / Encrypted)*
      * Secure isolated space for personal user data and configurations.
      * *Изолированное безопасное пространство для личных данных пользователей.*
    * **swap** — **≈1 GB** *(Logical Volume / Encrypted)*
      * Virtual memory partition used as an extension when physical RAM is fully utilized.
      * *Раздел виртуальной памяти, используемый при нехватке физической ОЗУ.*
    </details>
* **Disk type:** VDI (VirtualBox Disk Image).
* **Network (Сеть):** **NAT with Port Forwarding** — Essential for connecting from your host terminal to the guest VM via SSH (`Host Port: 4242` -> `Guest Port: 4242`).

#### Attaching ISO to VirtualBox
* **Select ISO:** Choose the downloaded ISO file.

### Step 3 🛠️ Installing VirtualBox
The most important part:
* **Set the hostname**, which must be the login followed by 42 (*onorina42*).
* **Domain name**: This section should be left blank since the subject doesn't require it.
* **Full name for the new user**: A new user that isn't the root user (*Olga Norina*).
* **Username**: A new user that isn't the root user, and the name for that user must be the student login (*onorina*).
* **Partitioning method**: Guided - use entire disk and set up encrypted LVM (*To fulfill the subject requirement "You must encrypt at least two partitions using LVM"*)
* **Choose software to install**: Nothing
* **GRUB Bootloader:** Installed directly to the primary drive (`/dev/sda`). *Required to allow the system to boot standalone and trigger the LUKS decryption screen. (загрузчик GRUB — маленькая программа, которая «оживляет» сервер при включении)*

### Step 4 📦 Installing sudo
1. Switch to root user
```
su
```
2. Install sudo package
```
apt install sudo
```
3. Reboot the system
```
sudo reboot
```
4. Verify the sudo installation
```
sudo -V
```

### Step 4 🧑‍💻 Creating a user and a group
```
sudo adduser <login>
```
```
sudo addgroup user42
```
```
sudo adduser <username> <groupname>
```
```
sudo adduser gemartin user42
```
```
sudo adduser gemartin sudo
```
```
getent group sudo user42
```
