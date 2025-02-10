# docker-demo

## local

```sh
docker login

# Build the Docker image
docker build -t fastapi-demo .

# Run the container
docker run -p 8000:8000 fastapi-demo
```

```sh
docker login
docker build --platform linux/amd64 -t fastapi-demo .
docker tag fastapi-demo rikwatson/fastapi-demo:tag
docker push rikwatson/fastapi-demo:latest
```

```sh
docker buildx build --platform linux/amd64,linux/arm64 \
  -t rikwatson/fastapi-demo:latest \
  --push .
```