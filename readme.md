# Multiple Dockerfiles and Docker Compose

- `context` is the directory from where we can copy files to Dockerfile.

---

### build docker compose up

```bash
docker compose -f docker-compose-dev.yml up
```

---

### Down Docker Compose, and also remove container and images

```bash
docker compose -f docker-compose-dev.yml down --rmi local # local only downs images not used by other containers (safer option)
``` 

---

### build docker compose but no-cache

```bash
docker compose -f docker-compose-dev.yml build --no-cache
```