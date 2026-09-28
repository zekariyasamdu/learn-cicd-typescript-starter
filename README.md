![alt text goes here](https://github.com/zekariyasamdu/learn-cicd-typescript-starter/actions/workflows/ci.yml/badge.svg)

# Note

- Build the Docker image locally:

```cmd
docker build -t DOCKERHUB_NAMESPACE/notely:latest .
```

- Run the Docker image locally

```cmd
docker run -e PORT=8080 -p 8080:8080 DOCKERHUB_NAMESPACE/notely:latest
```

- Build and push the Docker image to google's Artifact Registry:

```cmd
gcloud builds submit --tag REGION-docker.pkg.dev/PROJECT_ID/REPOSITORY/IMAGE:TAG .
```
