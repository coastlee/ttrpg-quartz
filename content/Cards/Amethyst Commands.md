---
tag: reference
---

up:: [[Linux]]

# Amethyst Commands

## Docker

- `docker ps -a`
    - shows all active containers
- `docker attach valheim.service`
    - see terminal logs of container
    - `CTRL+p` plus `CTRL+q` will exit the docker container without shutting it down

- `docker logs -f <CONTAINER>`
    - another option for seeing logs 

I'm having an issue where all docker commands are hanging. Perhaps that's contributing to not being able to access the valheim server.

Check out [this link](https://forums.docker.com/t/what-to-do-when-all-docker-commands-hang/28103) for resolving it later.



## Moving Files via `.ssh`

```bash
scp <source> <destination>
```

To copy a file from `B` to `A` while logged into `B`:

```bash
scp /path/to/file username@a:/path/to/destination
```

To copy a file from `B` to `A` while logged into `A`:

```bash
scp username@b:/path/to/file /path/to/destination
```