# HW4. Основы криптографической защиты информации

## Задание:

📌 1. Выполнить следующие задания семинара с операционными системами:

++ **_Задание №3. Расчет и проверка хэшей. Файл_**

Рассчитать хэш SHA-2 (длина хэша 256) для файла с использованием встроенных средств

Windows:

- в командной строке: `certutil -hashfile "путь к файлу" SHA256`;
- в PowerShell-оболочке: `get-filehash -Algorithm SHA256 "путь к файлу"`.

Linux:

- `sha256sum "путь к файлу"`.

++ **_Задание №3.2 Расчет и проверка хэшей. Строка_**

Рассчитать хэш SHA-2 (длина хэша 256) для текста («test»):

- в командной строке Windows:

  `echo|set /p="test" > %TMP%/hash.txt |certutil -hashfile %TMP%/hash.txt SHA256 | findstr /v "hash"`

- Linux:

  `echo -n test | sha256sum`

++ **_Проверить полученные значения хэшей в заданиях 3 и 3.2 на веб-ресурсах_**

---

📌 2. Доп. задание\* (не обязательное): напишите программу на Python, которая будет вычислять хэш-значения (файл формата .py или .ipynb).

---

_1. Выполнение задания №3:_

![hw4_img1](/hw4/img4/img4.1.jpg)

Проверка полученные значения хэшей на веб-ресурсах:

<https://hash-file.online>

<https://www.strerr.com/ru/sha256_file.html>

![hw4_img2](/hw4/img4/img4.2.jpg)

![hw4_img3](/hw4/img4/img4.3.jpg)

---

_2. Выполнение задания №3.2:_

![hw4_img4](/hw4/img4/img4.4.jpg)

Проверка полученные значения хэшей на веб-ресурсах:

<https://pi7.org/hash/sha256>

<https://md5decrypt.net/en/Sha256/>

![hw4_img5](/hw4/img4/img4.5.jpg)

![hw4_img6](/hw4/img4/img4.6.jpg)

---

_3. Выполнение доп.задания\*:_

Read more JupyterLab file [here get_hash_python.ipynb](./get_hash_python.ipynb)

<!-- Read more Python file [here get_hash_python.py](./get_hash_python.py)  -->
