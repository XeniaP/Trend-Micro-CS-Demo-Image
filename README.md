# TrendAI Code Security Scan Demo

This is a Docker Image used Only for Demostration - NOT USE IN PRODUCTION ENVIRONMENT

The main objective is to demonstrate the detection of Vulnerabilities, Malware and Some additional elements within a Pipeline.

How-to-use
1) Copy the project in your local environment
´´´
git clone https://github.com/XeniaP/Trend-Micro-Smart-Check-Demo-Image.git
cd Trend-Micro-Smart-Check-Demo-Image
´´´

2) Build image 
docker build -t demo-app:v1 .

3) Push your image in your Registry (ECR, ACR, GCR) - For this Example we use DockerHub [DockerHub](https://hub.docker.com/)
> you need to be logged into the Docker Registry, you can use the following commanand. $ docker login 

```
# tag your image
docker tag <your_repository_name>/demo-app:v1 demo-app:v1
# push your image
docker push <your_repository_name>/demo-app:v1
```

4) Perfect!, now you can scan this image with [Deep Security Smart Check](https://cloudone.trendmicro.com/docs/container-security/sc-about/)

----------------------------------------

## TO-DO

- [x] how-to build/upload image to registry
- [ ] how-to deploy Kubernetes
- [ ] how-to deploy Trend Micro Smart Check

## Contributing
If you encounter a bug, think of a useful feature, or find something confusing in the docs, please create a new issue!
We ❤️ pull requests.
