
```
docker run -d ubuntu 
```


Run in background
```
docker run -d ubuntu sleep 10000
```


List of container running
```
docker container ls 
```


To fix the the error permission of docker
```
cat /etc/subuid
```

```
grep "$USER" /etc/subuid >> /dev/null 2&>1 || (echo "$USER:100000:65536" | sudo tee -a /etc/subuid)
```
ref: https://docs.docker.com/desktop/faqs/linuxfaqs/
