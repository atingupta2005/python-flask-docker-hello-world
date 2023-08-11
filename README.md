# Simple Python Flask Dockerized Application

### Clone this repo
```
ssh atingupta2005@172.190.40.220
clear
cd
git clone https://github.com/atingupta2005/python-flask-docker-hello-world
cd ~/python-flask-docker-hello-world
```

### Review the files
```
clear
cd ~/python-flask-docker-hello-world
cat app.py
cat requirements.txt
cat Dockerfile
```

### Build the image using the following command

```bash
cd ~/python-flask-docker-hello-world
docker images
docker build -t simple-flask-app:latest .
docker images
```

### Run the Docker container using the command shown below.

```bash
docker container ls
docker run --name simple-flask-app-c -d -p 5000:5000 simple-flask-app
docker container ls
```

### Note
- The application will be accessible at:
      - http://172.190.40.220:5000


### Cleanup
```
docker container rm -f simple-flask-app-c
docker rmi simple-flask-app:latest
docker container ls
docker images
```
