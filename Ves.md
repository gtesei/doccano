# Docker - build image - Ves 

## build image 

```bash
docker build -f .\Dockerfile -t my_doccano_img .
```

## run image on host port 9000 


-p <host_port>:<container_port> 

```bash
docker run -d --name my_doccano -p 9000:8000 my_doccano_img
```


## run script to create admin uaser 

docker exec my_doccano tools/create-admin.sh "admin" "admin@example.com" "password"






