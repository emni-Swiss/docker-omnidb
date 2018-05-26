# OmniDB
OmniDB 2.8.0 on openSUSE Leap 15.0

[OmniDB](https://www.omnidb.org/en/) is a browser-based tool that simplifies database management focusing on interactivity, designed to be powerful and lightweight.

# Prepare the environment
```bash
mkdir -p /serverdata/wwwdata/_config/_omnidb
docker pull emni/omnidb
```
# Running
for testing
```bash
docker run --name omnidb -it --rm \
  -p 9336:8080 \
  -p 25482:25482 \
  -v /serverdata/wwwdata/_config/_omnidb:/data \
  emni/omnidb
```
for operation
```bash
docker run --name omnidb -d \
  -p 9336:8080 \
  -p 25482:25482 \
  -v /serverdata/wwwdata/_config/_omnidb:/data \
  emni/omnidb
```
# Login
Open [http://localhost:9336](http://localhost:9336)

Default login username: "admin" and password "admin".

