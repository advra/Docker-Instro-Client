# Instro Client Environment

Image file contianing the needed dependencies for developing and running the client. This environment serves as the gRPC client.

* gRPC
* Protobuf

### Step 1: Obtain docker images
```
docker pull asdfadrian/instro-client
```
### Step 2: Obtain hash id
```
docker images
```
The output should look like:
```
PS C:\Users\aaa> docker images
REPOSITORY                 TAG       IMAGE ID       CREATED        SIZE
asdfadrian/ubuntu-grpc     latest    91770c06a4cf   3 months ago   2.15GB
```
### Step 3: Run container using the hash Image ID tag from previous step  
```
docker run -it 91770c06a4cf bash 
```

# helpful docker commands
```
docker images                         // list all images
docker -ps -a                         // list all containers
docker run -it [containerhash] bash   // run container 
docker start [container]
docker stop [container]
```


## Other notes:

Alternatively you may use VSCode gui to perform the above steps. You will need to install the following:
- Vscode
- Remote Containers
- Remote SSH
- Remote WSL
- Remote Development
