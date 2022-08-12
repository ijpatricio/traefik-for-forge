
Step 1. Deploy Script
```
cd /home/forge/traefik
git pull origin $FORGE_SITE_BRANCH

docker-compose up -d --remove-orphans
```

Step 2. Configure ENV variables, and set Traefik Dashboard password
!!! Recommended doing via SSH, even you could fdo it from Forge's UI "Run command"
```
./Taskfile copyEnv
./Taskfile auth username password

```
