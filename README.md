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


'''
пользователи:
rabbitmqctl list_users
rabbitmqctl add_user test test
rabbitmqctl set_user_tags test administrator
rabbitmqctl set_permissions -p / test ".*" ".*" ".*"

политика репликации:
rabbitmqctl set_policy ha-all "" '{"ha-mode":"all","ha-sync-mode":"automatic"}'
'''