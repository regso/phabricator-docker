# phabricator-docker
Docker image for Phabricator

Install
-----
- Install docker (CE - Community Edition)
- Install docker-compose (CE - Community Edition)
- Restart system
- Check ```docker -v && docker-compose -v```
- Set permissions
```
sudo groupadd docker
sudo usermod -aG docker $USER
sudo chmod +x /usr/local/bin/docker-compose
```

Run
-----
`docker-compose up --build`

Rebuild images
`docker-compose build` or `docker-compose up --build`

Next steps
-----
- Running nginx in read-only mode https://hub.docker.com/_/nginx?tab=description
- Running nginx as a non-root user https://hub.docker.com/_/nginx?tab=description