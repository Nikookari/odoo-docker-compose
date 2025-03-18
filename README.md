# odoo-docker

This project prepared for implementing odoo by only one command.

**Rebuild and Run Container**

```
chmod +x entrypoint.sh wait-for-psql.py && docker-compose up --build
```

**Remove all data associated with Docker container**

```
docker-compose down
docker-compose down -v
docker rmi odoo-docker-odoo
docker volume prune -f
docker network prune -f
chmod +x entrypoint.sh wait-for-psql.py && docker-compose up --build
```
