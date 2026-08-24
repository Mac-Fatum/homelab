# Ubuntu — SIEM-сервер (Wazuh)

## IP-адреса
- Внутренняя сеть: `10.10.10.5`
- Сетевой мост: `192.168.0.28`

## Установленные компоненты
- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard

## Команды установки
```bash
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo gpg --dearmor | sudo tee /usr/share/keyrings/wazuh.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/wazuh.gpg] https://packages.wazuh.com/4.x/apt/ stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list
sudo apt update
sudo apt install wazuh-manager wazuh-indexer wazuh-dashboard -y

## Генерация сертификатов
cd /usr/share/wazuh-indexer/plugins/opensearch-security/tools/
sudo ./wazuh-certs-tool.sh -A
sudo cp /tmp/wazuh-certificates/* /etc/wazuh-indexer/certs/
