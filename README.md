# Prepare the environment
```bash
mkdir -p /serverdata/wwwdata/_config/_omnidb
```
# Running
```bash
docker run --name omnidb -it --rm -p 9336:8080 \
  -v /serverdata/wwwdata/_config/_omnidb:/data \
  emni/omnidb
```
# Login
Open [http://localhost:9336](http://localhost:9336)

Default login username: "admin" and password "admin".
