# Launch Redis cluster via docker-compose for local development purpose

This repo is cloned from: https://github.com/yowko/docker-compose-redis-cluster, here're some changes to fit my own needs:
1. Upgrade Redis version by using image `6.0.7-alpine`
2. Simplify the usage by removing the master/slave password (CAUTION: DO NOT USE IT ON PRODUCTION ENVIRONMENT)

## Prerequisites
- docker
- docker-compose


## Usage
#### Start Redis cluster
```bash
ip=$(ipconfig getifaddr en0) docker-compose up -d --build
```
The redis cluster will be ready on `127.0.0.1:7000`

#### Stop Redis cluster
```bash
 docker-compose down -v
```

