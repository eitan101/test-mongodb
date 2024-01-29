# test-mongodb

compose file is taken from [here](https://medium.com/workleap/the-only-local-mongodb-replica-set-with-docker-compose-guide-youll-ever-need-2f0b74dd8384)

test it using

```sh
git clone https://github.com/eitan101/test-mongodb.git
cd test-mongodb
docker compose up --wait
docker compose exec -it  mongo1 mongosh --eval "rs.status()"
```

The connection string is:

```
mongodb://127.0.0.1:27017,127.0.0.1:27018,127.0.0.1:27019/?replicaSet=rs0
```
