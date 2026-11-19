#!/usr/bin/env bash
# ==============================================================================
# SaviorBill Universal Installer Launcher
# https://get.saviorbill.com
# ==============================================================================
set -euo pipefail

# Если запуск через пайп (curl ... | bash), перенаправляем stdin на tty
if [ ! -t 0 ] && [ -e /dev/tty ]; then
  exec < /dev/tty
fi

INSTALL_DIR="${SAVIORBILL_DIR:-/opt/saviorbill}"
RAW_URL="https://raw.githubusercontent.com/UNVISLATE/SaviorBill/master/deploy/setup.sh"

echo "ℹ [SaviorBill] Загрузка актуального мастера развертывания..."

if [ ! -d "$INSTALL_DIR" ]; then
  if [ "${EUID:-$(id -u)}" -ne 0 ] && command -v sudo >/dev/null 2>&1; then
    sudo mkdir -p "$INSTALL_DIR"
    sudo chown -R "$(id -u):$(id -g)" "$INSTALL_DIR"
  else
    mkdir -p "$INSTALL_DIR"
  fi
fi

cd "$INSTALL_DIR" || exit 1

# Скачиваем и сохраняем локально в /opt/saviorbill/setup.sh
if command -v curl >/dev/null 2>&1; then
  curl -fsSL "$RAW_URL" -o "$INSTALL_DIR/setup.sh"
elif command -v wget >/dev/null 2>&1; then
  wget -qO "$INSTALL_DIR/setup.sh" "$RAW_URL"
else
  echo "✖ Ошибка: для продолжения требуется curl или wget в системе." >&2
  exit 1
fi

chmod +x "$INSTALL_DIR/setup.sh"
exec "$INSTALL_DIR/setup.sh" "$@"
