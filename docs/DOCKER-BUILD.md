# PgOSM-Flex Docker

Notes covering Docker and generating image for Docker Hub.  Most users will
not need this documentation!

----

Uses [main Postgres image](https://hub.docker.com/_/postgres/) via the [main PostGIS image](https://hub.docker.com/r/postgis/postgis) as starting point, see that
repo for full instructions on using the core Postgres functionality.

Build latest.

```bash
docker build -t rustprooflabs/pgosm-flex .
```


Tag with version.

```bash
docker build -t rustprooflabs/pgosm-flex:0.3.4 .
```

Push to Docker Hub.

```bash
docker push rustprooflabs/pgosm-flex:0.3.4
docker push rustprooflabs/pgosm-flex:latest
```
