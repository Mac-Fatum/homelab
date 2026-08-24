
---

#### `Windows-Target/README.md`


# Windows — целевая машина (жертва)

## IP-адрес
- Внутренняя сеть: `10.10.10.4`

## Установленные компоненты
- Wazuh Agent (подключён к `10.10.10.5`)
- Sysmon (для детального логирования)

## Установка Wazuh Agent
1. Скачать `.msi` с https://packages.wazuh.com/4.x/windows/
2. Установить, указав IP сервера: `10.10.10.5`

## Настройка Sysmon
```cmd
sysmon -accepteula -i
