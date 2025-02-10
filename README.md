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

docker tag fastapi-demo rikwatson/fastapi-demo:tag
docker push rikwatson/fastapi-demo:latest
```