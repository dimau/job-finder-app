# Job Finder Application
Docker-application dedicated to finding right job for the people

## Start Application in Dev Environment
#### Clone repositories for all microservices
```
git clone git@github.com:dimau/job-finder-app.git
git clone git@github.com:dimau/hh-collector.git
git clone git@github.com:dimau/telegram-collector.git
git clone git@github.com:dimau/hh-api-client-go.git
```
#### Run supporting third party services (Postgres, RabbitMQ...)
```
cd job-finder-app
docker compose up -d
```
#### Run hh-collector (optional)
```
docker compose -f docker-compose.hh-collector.yml build
docker compose -f docker-compose.hh-collector.yml up 
```

## Start Application in Prod Environment
```
git clone git@github.com:dimau/job-finder-app.git
cd job-finder-app
docker compose build
docker compose up -f docker-compose.yml -f docker-compose.prod.yml -d
```