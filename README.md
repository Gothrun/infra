# Infrastructure & DevOps Stack 🏗️

Репозиторий, содержащий конфигурацию и настройку инфраструктуры (Infrastructure as Code) для развертывания, управления и мониторинга микросервисов (Telegram-ботов).

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Uptime Kuma](https://img.shields.io/badge/Uptime_Kuma-5CDD8B?style=flat-square&logo=uptime-kuma&logoColor=black)

---

## 📖 О проекте
Данный репозиторий содержит `docker-compose.yml` для быстрого развертывания полноценного стека мониторинга и управления контейнерами на чистом Linux-сервере. 

Все сервисы запускаются в изолированной Docker-сети и имеют защищенные тома для хранения данных.

### 🛠 Компоненты системы:
*   **Portainer** — веб-интерфейс для управления Docker-контейнерами, образами и сетями.
*   **Prometheus** — система сбора и хранения метрик.
*   **Node Exporter** — агент для сбора метрик с хост-системы (CPU, RAM, диски).
*   **Grafana** — визуализация метрик, построение дашбордов и настройка алертов.
*   **Uptime Kuma** — мониторинг доступности сервисов (ping/HTTP), отправка уведомлений при падении.

## 📸 Демонстрация работы
<!-- ПЕРЕТАЩИ СЮДА СКРИНШОТ PORTAINER (список контейнеров) -->
<img width="1906" height="851" alt="image" src="https://github.com/user-attachments/assets/290c4a10-8c9f-49b8-9ec5-7222f7e76bdb" />


<!-- ПЕРЕТАЩИ СЮДА СКРИНШОТ GRAFANA (графики) -->
<img width="1911" height="880" alt="image" src="https://github.com/user-attachments/assets/044cdcb3-9a01-4106-b2bf-ef54642f6383" />


<!-- ПЕРЕТАЩИ СЮДА СКРИНШОТ UPTIME KUMA -->
<img width="1886" height="868" alt="image" src="https://github.com/user-attachments/assets/041f9064-08c5-4834-8d59-a0fac7776616" />


## 🚀 Развертывание инфраструктуры

### Требования:
*   Установленный Docker и Docker Compose.
*   Открытые порты (9000, 3000, 9090, 3001) или настроенный Reverse Proxy (Nginx/Traefik).

### Установка:
1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/Gothrun/infra.git
   cd infra
