FROM redis:6.0.7-alpine

COPY rediscluster.conf /etc/redis/rediscluster.conf

ENTRYPOINT redis-server /etc/redis/rediscluster.conf
