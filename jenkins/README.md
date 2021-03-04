Workflow pipeline:


<img width="480" alt="Diagram" src="https://user-images.githubusercontent.com/47504700/109980536-a2ffb280-7cc5-11eb-9b4a-61dd1a673a51.png">



#Prerequisites: 
- Kubernetes and Docker installed
- User needs Docker permissions

#Go into cloned repo directory after the clone command
```
cd myrepo
```

#Build image with the name myapp
```
docker build -t myapp ./
```

#Deploy and expose the services "prod, dev or qa"
```
kubectl apply -f yamls/<env>.yaml
```

#Example
```
kubectl apply -f yamls/dev.yaml
```

#Check what is runnig in Kubernetes, output will show you all the services/pods running
```
kubectl get all
```
