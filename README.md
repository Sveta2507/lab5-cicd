# ЛР 5. CI/CD

Проєкт для лабораторної роботи 5: HTML/CSS застосунок, Dockerfile та GitHub Actions pipeline, який перевіряє код, збирає Docker image і публікує його в Docker Hub.

## Локальний запуск

```powershell
docker build -t lab5-cicd-app .
docker run -d --name lab5-cicd-app -p 8080:80 lab5-cicd-app
```

Відкрити:

```text
http://localhost:8080
```

## GitHub Secrets

У репозиторії GitHub потрібно додати:

```text
DOCKERHUB_USERNAME
DOCKERHUB_TOKEN
```

## Image name

Pipeline публікує image у Docker Hub:

```text
DOCKERHUB_USERNAME/lab5-cicd-app:latest
```
