# Python boilerplate
Minimal setup for building a Python API running with Flask and MongoDB, inside Docker Containers. You can use FastAPI instead of Flask.

## Running it
```
docker-compose up --build -d
```

## Testing it
test endpoints:
```bash
curl localhost:5000/ping  # pong
curl localhost:5000/users  # Retrieves all users
curl --data "name=Yoonje Choi"  localhost:5000/users  # Adds new "username" user
```
unit testing
```bash
make test
``` 
