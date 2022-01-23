## Challenge 1

Build a image with the app.

#### Steps

- Go to src

``` bash
cd src
```

- Build the image describe in dockerfile

```bash
docker image build  -t your_usename/app_name:version .
```

- Run your app

```bash
docker container run -d -p 8080:8080 your_usename/app_name:version
```

#### Samples

- Docker image

![Docker image](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/docker-image.PNG?raw=true)

- Docker container

![Docker container](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/docker-contianer.PNG?raw=true)

- Application

![Application](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/running-app.PNG?raw=true)


## Challenge 2

#### Kubernets Deploy

- page

![Kubernets Deploy](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/kubernets-deploy.PNG?raw=true)

#### Setup

- K3D

```bash
choco install k3d
```

- kubernetes-cli

```bash
choco install kubernetes-cli
```

#### Scripts

- Create Cluster

```bash
k3d cluster create kube-cluster --servers 3 --agents 3 -p "8080:30000@loadbalancer"
```
- Run deployment

```bash
kubectl apply -f k8s/deployment.yaml
```


## Challenge 3

#### Kubernets Deploy

- page

![github-actions](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/github-actions.jpg?raw=true)

