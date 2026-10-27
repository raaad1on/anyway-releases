# Anyway Proxy

Бета **0.2.3-r1**. Пакеты для ImmortalWrt 25.12.x (`rockchip/armv8` / `aarch64_generic`).

- [Releases](https://github.com/raaad1on/anyway-releases/releases)
- Каталог [`packages/`](./packages) — `.apk` текущей беты
- APK feed: [`feed/packages.adb`](./feed/packages.adb)

## Установка / обновление

```sh
# one-time: add feed
echo 'https://raw.githubusercontent.com/raaad1on/anyway-releases/main/feed/packages.adb' \
  > /etc/apk/repositories.d/anyway.list
apk update --allow-untrusted
apk add --allow-untrusted anyway-xray luci-app-anyway-proxy

# later upgrades
apk update --allow-untrusted
apk upgrade --allow-untrusted anyway-xray luci-app-anyway-proxy
```

Или в LuCI → Anyway Proxy → Settings → **Update packages**.
