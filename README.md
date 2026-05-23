# 🕐 Clock App

A minimal, elegant web app that displays the current time and date.

## Files

```
app/
├── index.html          # The web app
├── Dockerfile          # Docker image definition
├── docker-compose.yml  # Easy run config
└── README.md
```

## Run with Docker Compose (recommended)

```bash
docker-compose up --build
```

Then open → http://localhost:8080

## Run with plain Docker

```bash
# Build the image
docker build -t clock-app .

# Run the container
docker run -d -p 8080:80 --name clock-app clock-app
```

Then open → http://localhost:8080

## Stop

```bash
# With docker-compose
docker-compose down

# With plain docker
docker stop clock-app && docker rm clock-app
```
