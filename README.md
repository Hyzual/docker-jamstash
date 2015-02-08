# docker-jamstash

A Dockerfile for [Jamstash](http://jamstash.com). Uses nginx.

Use the following command to run it on port 8001 of your host machine :

```bash
sudo docker run -d --name jamstash -p 8001:80 hyzual/jamstash
```

You can now connect to `http://yourhost:8001` and enjoy Jamstash.

## Ports

### 80

Web app port
