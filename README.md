# docker-pgpool

PGPool2 3.7.5 at debian9 docker image

## Quick start

```bash
docker run -it --rm -v $(pwd)/pgpool.conf:/etc/pgpool/pgpool.conf smirart/pgpool:latest
```

```bash
docker-compose up -d
```

pgpool needs three configuration files: `pgpool.conf`, `pcp.conf`, `pool_hba.conf`. You can add your own conf-file to `/etc/pgpool/` directory before use and `docker-entrypoint` will load that. Otherwise will be used standart configurations.
