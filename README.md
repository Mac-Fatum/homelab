# Home Lab - Purple Team

Домашняя лаборатория для отработки навыков обнаружения и реагирования на атаки

## Архитектура
- 3 виртуальные машины: Parrot (Attacker), Windows (Target), Ubuntu (SIEM)
- Внутренняя сеть 'homelab (10.10.10.0/24)'
- Wazuh SIEM (Manager + Indexer + Dashboard)

## Статус
- [x] UBUNTU-siem настроен
- [x] Wazuh Indexer работает
- [x] Wazuh Dashboard доступен
- [ ] Windows-агент установлен и подключен
- [ ] Sysmon настроен
- [ ] Тестовая атака проведена
