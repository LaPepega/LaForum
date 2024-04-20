FROM redis

EXPOSE 6379:6379

COPY redis.conf /usr/local/etc/redis/redis.conf

# No array syntax allows for env variables but breaks ctrl-c interupts
CMD redis-server /usr/local/etc/redis/redis.conf --requirepass ${REDIS_PASSWORD}