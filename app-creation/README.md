# App Creation using Jenkins X

### Create Sample Spring Boot App

https://jenkins-x.io/demos/create_spring/

```sh
$ jx create spring
```

Git repository created
selected pack: C:\Users\mac\.jx\draft\packs\github.com\jenkins-x-buildpacks\jenkins-x-kubernetes\packs\maven
replacing placeholders in directory D:\projects\MyJxSpringBoot
app name: myjxspringboot, git server: github.com, org: tomvmac, Docker registry org: tomvmac
skipping directory "D:\\projects\\MyJxSpringBoot\\.git"
skipping ignored file "D:\\projects\\MyJxSpringBoot\\HELP.md"
Pushed Git repository to https://github.com/tomvmac/MyJxSpringBoot
Let's ensure that we have an ECR repository for the Docker image tomvmac/myjxspringboot
Created ECR repository: 351073549249.dkr.ecr.us-east-2.amazonaws.com/tomvmac/myjxspringboot
Creating GitHub webhook for tomvmac/MyJxSpringBoot for url http://hook.jx.aea9576d496c011e9bc170ac7325003f-9c7109bbf5eba00b.elb.us-west-2.amazonaws.com/hook

Watch pipeline activity via:    jx get activity -f MyJxSpringBoot -w
Browse the pipeline log via:    jx get build logs tomvmac/MyJxSpringBoot/master
You can list the pipelines via: jx get pipelines
When the pipeline is complete:  jx get applications

For more help on available commands see: https://jenkins-x.io/developing/browsing/

Note that your first pipeline may take a few minutes to start while the necessary images get downloaded!