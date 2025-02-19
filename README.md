# Todo App Docker
If you want to embed images, this is how you do it:  

<!--![Demo](todo-list-sample.png)-->
<img src="nodejs-todo-app.png" alt="drawing" height="400" />

## Commands  
**Build image from Dockerfile**
```
docker build -t nodejs-todo-app .
```

**Run container**
```
docker run -dp 3000:3000 --name=node-app nodejs-todo-app
```
**inspect container ipaddress**
```
docker inspect <container_id> 
```

**Execute commands inside a container**
```
docker exec -it <container_id> /bin/sh
```

**Execute Command for login to dockerhub via CLI**
```
docker login -u <dockerhub username>
```

**Push the Dockerfile to Dockerhub**
```
docker tag <source_image> <target_image>
```

```
docker push <dockerhubusername>/nodejs-todo-app:tagname
```

 
