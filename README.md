<div align="center">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/logo.png" width="120" height="120" style="border-radius: 24px">
  <h1>Whitelist Checker (Проверка ограничений интернета)</h1>

**Whitelist Checker** — Приложение для Android, предназначенное для автоматического мониторинга сетевого соединения на наличие ограничений провайдеров, а также их обхода через интеграцию со сторонними VPN-приложениями.
</div>
<div align="center">
  Рекомендуется использовать в связке с <a href="https://github.com/okhsunrog/vpnhide" target="_blank">VPN hide<a>
</div>
    
---

## 📸 Скриншоты

<div align="center">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/screenshots/photo_2026-07-05_13-12-03.jpg" width="200">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/screenshots/photo_2026-07-05_13-12-06.jpg" width="200">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/screenshots/photo_2026-07-05_13-12-09.jpg" width="200">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/screenshots/photo_2026-07-05_13-12-00.jpg" width="200">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/screenshots/photo_2026-07-05_13-11-56.jpg" width="200">
  <img src="https://raw.githubusercontent.com/UkolovArtem-dev/WhitelistChecker/refs/heads/main/assets/screenshots/photo_2026-07-05_13-11-49.jpg" width="200">
</div>

---

## 🛠 Ключевые возможности

### 🔍 Интеллектуальный мониторинг
*   **Обнаружение «Белых списков»:** Автоматическая проверка доступности ресурсов. Система определяет, ограничен ли доступ только разрешенным списком сайтов (Whitelist).
*   **Обнаружение Шейпа (Замедление интернета):** Встроенный алгоритм замера скорости позволяет выявлять искусственное ограничение пропускной способности канала (Shape).
*   **Мониторинг Wi-Fi и Мобильной сети:** Раздельные сценарии поведения для разных типов подключения.

### 🤖 Автоматизация VPN
*   **Динамическое переключение:** Автоматический запуск выбранного VPN-профиля при обнаружении белых списков или шейпа.
*   **Root-возможности:** Использование прав суперпользователя для управления Quick Settings плитками сторонних приложений и автоматического переключения VPN без участия пользователя.
*   **Intent-управление:** Гибкая настройка отправки широковещательных сообщений (Broadcast Intents) для глубокой интеграции с VPN-клиентами.

### 📊 Инструменты и интерфейс
*   **Информативный виджет:** Статус сети, обновление IP, скорость интернета и время до следующей проверки прямо на рабочем столе.
*   **Быстрые настройки (Tiles):** Мгновенная проверка доступности интернета через шторку уведомлений.
*   **Журналирование событий:** Подробный лог всех сетевых событий, смен IP и действий автоматики.
*   **Статистика:** Наглядные данные о доступности интернета.

### ⚙️ Кастомизация
*   **Планировщик:** Настройка «часов сна» для экономии заряда батареи и отключения автоматики в ночное время.
*   **Современный UI:** Интерфейс на Jetpack Compose с поддержкой динамических цветов, темной темы и настраиваемых акцентов.
*   **IP Refresh:** Функция автоматического обновления IP-адреса через GET-запрос к внешнему ресурсу при восстановлении связи.

---

## 🚀 Технологический стек
*   **Язык:** Kotlin
*   **UI:** Jetpack Compose (Material 3)
*   **Concurrency:** Kotlin Coroutines
*   **Background:** Android Services, Broadcast Receivers
*   **Persistence:** DataStore / SharedPreferences

---

## 📦 Установка и использование

1.  Скачайте актуальный APK из раздела [Releases](https://github.com/UkolovArtem-dev/WhitelistChecker/releases).
2.  Предоставьте необходимые разрешения (уведомления, доступ к состоянию телефона).
3.  Запустите службу.
4.  Для расширенных функций автоматизации (управление сторонними VPN) рекомендуется наличие **Root-прав**, однако базовый мониторинг работает на любых устройствах.
