X# Домашнє завдання №2
## Файлова система і права доступу

ПІБ: Черкасов Михайло Вячеславович

## Завдання 1. Ієрархія каталогів Linux

### Кореневий каталог /

Команди:

cd /
pwd
ls

Результат:

/
bin boot dev etc home lib lib64 media mnt opt proc root run sbin snap srv sys tmp usr var

### Каталог /etc

Команди:

cd /etc
pwd
ls

Результат:

/etc

(виведено список конфігураційних файлів та каталогів)

### Каталог /home

Команди:

cd /home
pwd
ls

Результат:

/home
micheal

---

## Завдання 2. Файли, каталоги та посилання

Команди:

cd ~
mkdir lab2
cd lab2

echo "This is my Linux homework file" > file.txt

cp file.txt file_copy.txt

mv file_copy.txt renamed_file.txt

ln file.txt hard_link_file.txt

ln -s file.txt symbolic_link_file.txt

find ~ -name "file.txt"

Результат:

/home/micheal/lab2/file.txt

Створено:
- file.txt
- renamed_file.txt
- hard_link_file.txt
- symbolic_link_file.txt

---

## Завдання 3. Права доступу

Команди:

ls -l file.txt

chmod 444 file.txt

chmod u+w file.txt

umask

umask 022

umask

Результат:

-rw-r--r-- 2 micheal micheal 31 Jun 20 14:48 file.txt

-r--r--r-- 2 micheal micheal 31 Jun 20 14:48 file.txt

-rw-r--r-- 2 micheal micheal 31 Jun 20 14:48 file.txt

0022

---

## Завдання 4. Користувачі

Команди:

sudo adduser trainee

sudo usermod -aG sudo trainee

grep trainee /etc/passwd

groups trainee

Результат:

trainee:x:1001:1001:,,,:/home/trainee:/bin/bash

trainee : trainee sudo users

---

## Висновок

Під час виконання роботи були відпрацьовані навички навігації файловою системою Linux, створення файлів і каталогів, роботи з жорсткими та символічними посиланнями, зміни прав доступу та створення користувачів.
