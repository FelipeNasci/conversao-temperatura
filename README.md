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

![](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/docker-image.PNG?raw=true)
![](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/docker-contianer.PNG?raw=true)
![](https://github.com/FelipeNasci/conversao-temperatura/blob/main/images/running-app.PNG?raw=true)
