# apisix-keycloak-docker-compose

* Run docker-compose 
  ```sh
  $ docker-compose up -d
  ```

* Keycloak URL:
http://localhost:8080/

* postgres:
localhost:5432
create database: keycloak

* Kafka
topic: apisix_logs

* Kafka-UI
http://localhost:9090/

* APISIX Dashboard URL:
http://localhost:9000/


*openrouter test
curl http://localhost:9080/chat/completions \
  -H "Authorization: Bearer YOUR_OPENROUTER_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "openai/gpt-3.5-turbo",
    "messages": [{"role": "user", "content": "Hello!"}]
  }'