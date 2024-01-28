# test-mongodb

compose file is taken from [here](https://medium.com/workleap/the-only-local-mongodb-replica-set-with-docker-compose-guide-youll-ever-need-2f0b74dd8384)

test it using

```sh
git clone https://github.com/eitan101/test-mongodb.git
cd test-mongodb
docker compose up --wait
docker compose exec -it  mongo1 mongosh --eval "rs.status()"
```
