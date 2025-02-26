# Xray Access View

**Xray Access View** — это утилита для анализа логов Xray, которая позволяет:

- **Анализ подключений:** Просматривать, какие домены и IP-адреса подключались под определённым Email.
- **Визуальное выделение:** Российские домены автоматически подсвечиваются красным.
- **Режим сводки:** Определять уникальные IP-адреса, ассоциированные с каждым Email.

---

## Особенности

- **Простой запуск:** Запустите скрипт напрямую из GitHub без предварительной установки.
- **Гибкость:** Укажите кастомный путь к логам или используйте путь по умолчанию (`/var/lib/marzban/access.log`).
- **Режимы отображения:**
  - **Основной режим:** Отображает список доменов и IP-адресов по каждому Email.
  - **Режим сводки:** С помощью параметра `--summary` выводит только уникальные IP-адреса для каждого Email.

---

## Установка и использование

#### Кастомный путь для логов
```
Укажите путь до логов (нажмите Enter для использования '/var/lib/marzban/access.log'): '/my/path/access.log'
```

### Запуск в основном режиме

```bash
python3 <(curl -sL https://github.com/Davoyan/xray-acess-view/raw/main/view.py)
```

### Запуск в режиме сводки

```bash
python3 <(curl -sL https://github.com/Davoyan/xray-acess-view/raw/main/view.py) --summary
```
