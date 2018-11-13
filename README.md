openstack client on python 2.7 (docker)
=======================================

run
---

**note:** you must have your openstack rc file located in `./creds.sh`, or 
update the `$(pwd)/creds.sh` below to match the desired path.

```bash
docker run -v $(pwd)/creds.sh:/creds.sh -ti pemcconnell/docker-openstack:latest
```



build
-----

You only need to do this if you want to build from source locally. This image is pulled from Docker Hub otherwise.

```bash
docker build -t=pemcconnell/docker-openstack:latest .
```
