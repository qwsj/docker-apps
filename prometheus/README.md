Prepare: 
```
mkdir -p prometheus/data grafana/data
chown nobody:nogroup prometheus/data
chown 472:472 grafana/data
```

Running:
```
. ./environment
docker-compose up -d
```