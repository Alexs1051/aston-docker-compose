# 8. DevOps

---

### Цель работы
Создать docker-compose.yml, который развернет всю микросервисную систему, включая Kafka, PostgreSQL, API Gateway, Service Discovery, External Configuration и 2 микросервиса(user-service и notification-service, созданные ранее). Проверить, что сервисы корректно взаимодействуют друг с другом в контейнерной среде.

### Результат
Таймкоды:
- 00:00-00:16 = запуск docker-compose
- 00:52-00:59 = падают сервисы user и notification (т.к. не успевает развернуться config-server)
- 00:59-01:03 = ручной перезапуск user и notification сервисов
- 01:07------- = запустилась eureka и api-gateway
- 01:11------- = запустился circuit-breaker
- 01:27------- = запустился config-server и notification-service
- 01:28-01:32 = демонстрация config-server
- 01:34------- = запустился user-service
- 01:35-01:43 = демонстрация работы user-service и notification-service
- 01:45-02:17 = тестовые запросы

https://github.com/user-attachments/assets/3b07db4d-8e2d-4889-a748-fc47e3fd3e49
