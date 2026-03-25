# Nexus-core: Infrastructure lab focused on DevOps technology stack
First things first, there's a reverse-proxy nginx webserver that you need to install on your machine and set like a daemon. The config of that reverse-proxy lies in "default" file, that you need to move/copy to /etc/nginx/sites-available/default on your server.

You can do that running something like that
```bash
sudo cp nginx/default /etc/nginx/sites-available/default
sudo systemctl restart nginx
```

And then deploy the stack:
```bash
docker compose up -d
```
