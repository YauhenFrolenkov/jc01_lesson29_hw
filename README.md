# Banking System Console Application. Final project.

Простое Java-приложение для управления банковскими счетами через консольный интерфейс. Построено по архитектуре MVC, 
реализует принципы чистой архитектуры, использует шаблоны проектирования и обрабатывает исключения на уровне сервиса и контроллера.


✅ **Основная функциональность:**

- 📄 Создание нового счета
- 💰 Пополнение счета (deposit)
- 🏧 Снятие средств (withdraw)
- 🔁 Перевод средств между счетами (transfer)
- 🔎 Получение всех счетов по email клиента
- ❌ Удаление счета

Все операции производятся через консольное меню, данные хранятся в текстовом файле `accounts.txt`.


🧱 **Архитектура:**

- `model` — бизнес-сущности:
  - `Account` — банковский счёт
  - `Client` — клиент банка
  - `Manager` — **зарезервирован для будущей функциональности (роль банковского менеджера, пока не используется в бизнес-логике)**
- `repository` — слой доступа к данным (работа с файлом)
- `service` — бизнес-логика (валидация, транзакции)
- `controller` — обработка текстовых команд
- `ui` — консольное меню (BankConsoleView)
- `util` — вспомогательные классы (валидация, операции)

⚙️ **Пример использования:**

```
==== Banking System Menu ====

Create Account
Deposit
Withdraw
Transfer
Get Client Accounts
Delete Account
Exit
```

🚀 **Возможности для расширения:**

- ✅ Хранение данных в базе данных (например, SQLite, PostgreSQL)
- 🔐 Аутентификация клиентов
- 📊 Вывод истории операций
- 🌐 Создание REST API с использованием Spring Boot
- 💻 GUI-интерфейс (JavaFX или Swing)
- 🧪 Покрытие кода модульными тестами (JUnit)

ℹ️ **Примечание:**  
Класс `Manager` на данный момент не используется в бизнес-логике, но добавлен в проект для возможной реализации ролевой модели доступа или административного функционала в будущем.
