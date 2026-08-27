# Home Lab — Purple Team

Домашняя лаборатория для отработки навыков обнаружения и реагирования на атаки.

## Архитектура
- 3 ВМ в VirtualBox
- Внутренняя сеть: `homelab` (10.10.10.0/24)
- Ubuntu — SIEM-сервер (Wazuh)
- Parrot — атакующая машина
- Windows — целевая машина с агентом Wazuh

## Доступ к дашборду
- `https://192.168.0.28` (IP сетевого моста)
- Логин/пароль сохранены локально

## Документация по машинам
- [Ubuntu (SIEM)](Ubuntu-SIEM/README.md)
- [Parrot (Attacker)](Parrot-Attacker/README.md)
- [Windows (Target)](Windows-Target/README.md)

## Статус
- [x] Сеть настроена
- [x] Wazuh установлен и работает
- [x] Windows-агент подключён
- [ ] Тестовая атака проведена
