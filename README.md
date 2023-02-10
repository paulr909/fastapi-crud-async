# FastAPI App

Build the images and run the containers:
```shell
docker-compose up -d --build
```

Run tests:
```shell
docker-compose exec web pytest .
```

Connect to database via psql:
```shell
docker-compose exec db psql --username=fastapi_user --dbname=fastapi_db
```

Test the routes:

- [http://localhost:8002/ping](http://localhost:8002/ping)
- [http://localhost:8002/docs](http://localhost:8002/docs)
- [http://localhost:8002/notes](http://localhost:8002/notes)
