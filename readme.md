# Python Web Homework 02

## Опис

Веб-застосунок на Python, який запускається разом із базою даних PostgreSQL у Docker-контейнерах за допомогою Docker Compose.

---

## 🚀 Швидкий старт

1. Клонуй цей репозиторій:

   ```bash
   git clone https://github.com/yuratouch/goit-pythonweb-hw-02.git
   ```

2. Запусти застосунок разом із базою командою:

   ```bash
   docker compose up --build
   ```

3. Відкрий у браузері:
   ```
   http://localhost:8000
   ```
   Головна сторінка та API будуть доступні після старту контейнерів.

---

## ⚙️ Структура проєкту

- **Dockerfile** — збирає образ застосунку Python 3.10
- **docker-compose.yaml** — піднімає сервіси `app` (застосунок) і `db` (PostgreSQL)
- **requirements.txt** — залежності Python
- **conf/db.py** — підключення до бази через сервіс `db`

---

## 🛠 Корисні команди

- Зупинити і видалити контейнери:
  ```
  docker compose down
  ```
- Для чистого старту видалити volume:
  ```
  docker compose down -v
  ```
- Після зміни залежностей — перебудувати:
  ```
  docker compose build
  ```

---
