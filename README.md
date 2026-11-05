# Storefront Site: Dockerized

A DevOps class exercise in containerizing a static website. The site is the free "Eflyer" e-commerce HTML template (fashion, electronics, and jewelry pages). My part was the Docker setup: packaging the site into an Apache httpd image and running it with Docker Compose.

## Files

```
Dockerfile           Copies the site into an Apache httpd 2.4 image
docker-compose.yml   Runs the container on port 80
*.html, css/, js/    The template
```

## Running it

```bash
docker build -t storefront .
docker run -p 8080:80 storefront
```

Then open http://localhost:8080.
