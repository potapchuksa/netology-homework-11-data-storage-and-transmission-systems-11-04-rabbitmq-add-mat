# RabbitMQ Код с лекции «Очереди RabbitMQ»


```
для запуска RabbitMQ переименуйте файл .env_example в .env и выполните:
- docker compose up -d (если используете docker compose версии > 2)
- docker-compose up -d (если используете docker compose версии < 2)
```


```
для запуска примеров из директории ./demo:
- cd demo
- python3 -m venv env
- source ./env/bin/activate
- pip install -r requirements.txt

- python consumer.py   - запуск консьюмера
- python producer_single.py    - запуск продюссера для отправки одного сообщения
- python producer.py     - запуск продюссера для отправки потока сообщений

```