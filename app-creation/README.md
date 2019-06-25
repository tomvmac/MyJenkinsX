# App Creation using Jenkins X

### Create Sample Spring Boot App

https://jenkins-x.io/demos/create_spring/

```sh
$ jx create spring
```

### Useful Commands:

Watch pipeline activity via:    jx get activity -f {appName} -w
Browse the pipeline log via:    jx get build logs tomvmac/{appName}/master
You can list the pipelines via: jx get pipelines
When the pipeline is complete:  jx get applications


```sh
$ jx get activity -f {appName} -w
$ jx get build logs
$ jx get applications
$ jx get env
$ jx get urls
```

### Code Pipeline Workflow:
1. Check out branch
2. Update, commit and push branch to origin
3. Intitiate Pull Request for branch code
4. Approve Pull Request 
5. Merge to Master



