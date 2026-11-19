# get.saviorbill.com

Официальный репозиторий раздачи оригинального инсталлятора **SaviorBill**.

### Быстрая установка

```bash
curl -fsSL https://get.saviorbill.com | bash
```

или альтернативный прямой вызов:

```bash
curl -fsSL https://get.saviorbill.com/setup.sh | bash
```

---

### Архитектура:
* Файл **`index.html`** содержит оригинальный исполняемый скрипт `deploy/setup.sh` из [SaviorBill](https://github.com/UNVISLATE/SaviorBill), что позволяет GitHub Pages отдавать скрипт по корневому адресу без `404`.
* Файл **`setup.sh`** — идентичная копия для прямых запросов.
* Скрипт автоматически гарантирует развертывание и работу стека строго в каталоге `/opt/saviorbill/`.
