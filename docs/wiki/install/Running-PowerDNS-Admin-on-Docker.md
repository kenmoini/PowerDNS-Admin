# Installation on docker

The Docker image is kenmoini/powerdns-admin available on [GitHub Container Registry](https://github.com/kenmoini/powerdns-admin/pkgs/container/powerdns-admin)

The supported environment variables to configure the container are located [here](../configuration/Environment-variables.md).

You can run the container and expose the web server on port 8080 using:
```bash
docker run -d \
    -e SECRET_KEY='a-very-secret-key' \
    -v pda-data:/data \
    -p 8080:80 \
    ghcr.io/kenmoini/powerdns-admin:latest
```
