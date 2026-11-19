# get.saviorbill.com

Универсальная точка входа для быстрой установки и развертывания биллинга **SaviorBill**.

### Использование

```bash
curl -fsSL https://get.saviorbill.com | bash
```

или альтернативный вариант:

```bash
curl -fsSL https://get.saviorbill.com/setup.sh | bash
```

### Как это устроено:
1. Запрос к `get.saviorbill.com` обрабатывается GitHub Pages.
2. Скрипт-загрузчик автоматически создаёт целевой каталог `/opt/saviorbill`.
3. Загружает самую свежую версию мастера развертывания `deploy/setup.sh` из репозитория [SaviorBill](https://github.com/UNVISLATE/SaviorBill).
4. Запускает интерактивный мастер установки в терминале.
