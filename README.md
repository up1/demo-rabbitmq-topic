## Start RabbitMQ Server

```
$docker container run -d --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
```

Admin page at `http://localhost:15672/`

- username=guest
- password=guest

## Start Consumer

```
$go run consumer-group.go g1
$go run consumer-group.go g1

$go run consumer-group.go g2
$go run consumer-group.go g2
```

## Start Producer

```
$go run producer-group.go <message>
```
