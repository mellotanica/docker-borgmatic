```
docker-borgmatic/
├── base
│   ├── data
│   │   └── borgmatic.d
│   │       ├── config.yml
│   │       └── crontab.txt
│   ├── docker-compose.restore.yml     
│   ├── docker-compose.yml
│   ├── Dockerfile
│   ├── entry.sh      
├── msmtp
│   ├── data
│   │   └── borgmatic.d
│   │       ├── config.yml             # same as in base
│   │       └── crontab.txt            # with mailto
│   │       └── msmtprc.sh
│   ├── docker-compose.yml             # image: mellotanica/borgmatic:latest-msmtp, env: msmtp.env
│   ├── Dockerfile                     # FROM mellotanica/borgmatic:${VERSION}
│   ├── entry.sh                       # starts msmtp in addition
│   └── README.md                      # describes specifics only
├── ntfy
│   ├── data
│   │   └── borgmatic.d
│   │       ├── config.yml             # same as in base
│   │       └── crontab.txt            # same as in base
│   ├── docker-compose.yml             # image: mellotanica/borgmatic:latest-ntfy
│   ├── Dockerfile                     # FROM mellotanica/borgmatic:${VERSION}
│   ├── entry.sh                       # same as in base
│   └── README.md                      # describes specifics only
└── README.md     
```
