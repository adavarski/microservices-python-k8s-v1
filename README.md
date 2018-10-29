App for the Microservices 

Edit services/config.yaml
```
AMQP_URI: amqp://${RABBIT_USER:guest}:${RABBIT_PASSWORD:guest}@${RABBIT_HOST:rabbitmq}:${RABBIT_PORT:5673}/
RABBIT_CTL_URI: http://guest:guest@rabbitmq:15673
WEB_SERVER_ADDRESS: '0.0.0.0:5000'
RPC_EXCHANGE: 'simplebank-rpc'
```
```
docker-compose --build
```
