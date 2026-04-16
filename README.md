# 🏦 Bank App (Fullstack Vanilla JS Project)

Полноценное банковское приложение с клиент-серверной архитектурой. Проект написал на "чистом" JavaScript без использования UI-фреймворков на фронтенде.

## 🚀 Основной функционал

*   **Auth System:** Полноценная авторизация на базе JWT-токенов. Реализовал безопасное хранение сессий и работа с Cookie.
*   **Transactions & Wallet:** 
    *   Перевод денежных средств между пользователями в реальном времени.
    *   Пополнение баланса и просмотр истории операций.
    *   Визуализация данных: интерактивный анимированный график транзакций.
*   **API Interaction:** Реализовал полный цикл CRUD-операций через REST API (GET, POST, PUT, DELETE).

## 🛠 Технологический стек

### Frontend (Vanilla JS)
*   **Language:** JavaScript (ES6+), Babel для поддержки старых браузеров.
*   **Styles:** SCSS с использованием BEM-методологии.
*   **Build Tool:** Кастомная сборка Webpack 5. Настроена минификация CSS (CSSMinimizer) и JS (Terser), а также оптимизация ассетов.
*   **Linting:** Конфигурация ESLint и Prettier.

### Backend (Node.js)
*   **Framework:** NestJS (TypeScript).
*   **Database:** PostgreSQL.
*   **ORM:** Prisma (с использованием миграций и типизации схем).
*   **Security:** Хеширование паролей (Argon2), JWT-стратегии (Passport.js).

*   **Client-Server Synchronization:** Самостоятельная настройка взаимодействия фронтенда с NestJS API.
*   **Data Visualization:** Реализация динамических графиков на чистом JS/Canvas без внешних библиотек.

## 📦 Запуск проекта

Проект состоит из двух частей. Для корректной работы необходимо запустить обе.

### 1. Backend (NestJS + PostgreSQL)
1. Установите зависимости: `npm install`
2. Настройте БД (Prisma): `npx prisma generate`
3. Запуск: `npm run start:dev`

### 2. Frontend (Webpack)
1. Установите зависимости: `npm install`
2. Запуск: `npm run dev`