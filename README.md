# Job Finder Application
Docker-application dedicated to finding right job for the people

## Start Application in Dev Environment
```
git clone git@github.com:dimau/job-finder-app.git
git clone git@github.com:dimau/job-collector-go.git
git clone git@github.com:dimau/telegram-bot-collector.git
git clone git@github.com:dimau/go-hh-client.git
cd job-finder-app
docker compose up -d
```

## Start Application in Prod Environment
```
git clone git@github.com:dimau/job-finder-app.git
cd job-finder-app
docker compose up -f docker-compose.yml -f docker-compose.prod.yml -d
```